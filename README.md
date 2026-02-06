# PDF/A-Compliant Guide

[NSF-PAR](https://par.nsf.gov/), among other, requires [PDF/A](https://en.wikipedia.org/wiki/PDF/A) documents.
They prodive [some indications](https://resources.research.gov/common/attachment/Desktop/How_do_I_create_a_PDF-A_file.pdf) on how to produce such documents, but unfortunately only using Microsoft Word Documents and Adobe Acrobat Professional.

## From a .tex source code

If you can access a `.tex` source code, then you can use [latex2pdfa](https://github.com/abdeladim-s/latex2pdfa).

## From a .pdf

If you can only access the `.pdf` (for example of the published version), then you can use [OCRmyPDF](https://github.com/ocrmypdf/OCRmyPDF), for example with 

```
ocrmypdf --tesseract-timeout=0 --skip-text input.pdf output.pdf
```

so that your document is not "OCRized".
