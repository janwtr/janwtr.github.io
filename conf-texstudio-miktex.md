# Konfigurasi TexStudio jika menggunkan MikTex

## Lingkungan
1. Sistem Operasi Windows 10
1. MiKTex (https://miktex.org/download)[https://miktex.org/download]
1. TeXstudio 2.12.22 (https://www.texstudio.org/)[https://www.texstudio.org/]

## konfigurasi pada TextStudio
1. LaTeX: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\miktex\texmfs\install\miktex\bin\latex.exe" -interaction=nonstopmode %.tex`
1. PdfLaTeX: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\x64\pdflatex.exe" -interaction=nonstopmode %.tex`
1. XeLaTeX: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\x64\xelatex.exe" -interaction=nonstopmode %.tex`
1. LuaLaTeX: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\x64\lualatex.exe" -interaction=nonstopmode %.tex`
1. Latexmk: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\x64\latexmk.exe" -e "$pdflatex=q\pdflatex -interaction=nonstopmode\" -pdf %.tex`
1. Bib(la)tex: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\x64\biber.exe" %`
1. Makeindex: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\x64\makeindex.exe" %.idx`
1. dvips: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\x64\dvips.exe" -o %.ps %.dvi`
1. Dvipdfm: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\x64\dvipdfm.exe" %.dvi`
1. ps2pdf: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\x64\ps2pdf.exe" %.ps`
1. metapost: `"D:\LaTeX\MikTex\bin\x64\mpost.exe" –interaction nonstopmode`
1. Asymptote: `"C:\Program Files\Asymptote\asy.exe" %.asy`
1. ghostscript: `"C:\Program Files\gs\gs9.07\bin\gswin32c.exe"`
1. R Sweave: `"..\R\bin\R.exe" CMD Sweave %.Rnw`
1. Dvi Viewer: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\x64\yap.exe" -1 -s @%.tex %.dvi`
1. PS Viewer: `"C:\Program Files\Ghostgum\gsview\gsview32.exe" %.ps (optional: Click the Embed checkbox)`
