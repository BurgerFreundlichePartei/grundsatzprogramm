
```bash
pandoc Satzung.md \
--standalone --toc --toc-depth=2 --number-sections \
--metadata pagetitle="Satzung der BFREI" -V lang=de \
--css bfrei-print.css \
--pdf-engine=wkhtmltopdf \
--pdf-engine-opt=--print-media-type \
--pdf-engine-opt=--enable-local-file-access \
--pdf-engine-opt=--footer-center="Satzung BFREI — [page]/[toPage]" \
-o Satzung_BFREI_barrierefrei.pdf
```
```bash
pandoc Satzung.md \
--standalone --toc --number-sections \
--metadata pagetitle="Satzung der BFREI" -V lang=de \
--css bfrei-print.css \
--pdf-engine=xelatex \
-V mainfont="DejaVu Serif" \
--pdf-engine-opt=--print-media-type \
--pdf-engine-opt=--enable-local-file-access \
--pdf-engine-opt=--footer-center="Satzung BFREI — [page]/[toPage]" \
-o Satzung_BFREI_barrierefrei.pdf
```
```bash
pandoc Satzung.md \
--standalone --toc --toc-depth=2 --number-sections \
--metadata title="Satzung der BFREI" -V lang=de \
--css bfrei-print.css \
--pdf-engine=weasyprint \
-o Satzung_BFREI_barrierefrei.pdf
```
