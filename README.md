# compress_pdf
Command to compress a pdf file

gs -sDEVICE=pdfwrite -dCompatibilityLevel=1.4 -dPDFSETTINGS=/ebook -dNOPAUSE -dQUIET -dBATCH -dColorImageResolution=150 -sOutputFile=output.pdf input.pdf


- -dPDFSETTINGS=/screen lower quality, smaller size. (72 dpi)
- -dPDFSETTINGS=/ebook for better quality, but slightly larger pdfs. (150 dpi)
- -dPDFSETTINGS=/prepress output similar to Acrobat Distiller "Prepress Optimized" setting (300 dpi)
- -dPDFSETTINGS=/printer selects output similar to the Acrobat Distiller "Print Optimized" setting (300 dpi)
- -dPDFSETTINGS=/default selects output intended to be useful across a wide variety of uses, possibly at the expense of a larger output file

use -dColorImageResolution obtion to tweek small adjustments.
