## Lingkungan
1. Sistem Operasi Windows 10
1. MiKTex (https://miktex.org/download)[https://miktex.org/download]
1. TeXstudio 2.12.22 (https://www.texstudio.org/)[https://www.texstudio.org/]

## konfigurasi pada TextStudio
1. LaTeX: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\miktex\texmfs\install\miktex\bin\latex.exe" -interaction=nonstopmode %.tex`
1. PdfLaTeX: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\pdflatex.exe" -interaction=nonstopmode %.tex`
1. XeLaTeX: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\xelatex.exe" -interaction=nonstopmode %.tex`
1. LuaLaTeX: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\lualatex.exe" -interaction=nonstopmode %.tex`
1. Dvi Viewer: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\yap.exe" -1 -s @%.tex %.dvi`
1. PS Viewer: `"C:\Program Files\Ghostgum\gsview\gsview32.exe" %.ps (optional: Click the Embed checkbox)`
1. Eternal PDV Viewer: <default>
1. dvips: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\dvips.exe" -o %.ps %.dvi`
1. dviPng:
1. ps2pdf: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\ps2pdf.exe" %.ps`
1. dviPdf: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\dvipdfm.exe" %.dvi`
1. BibTex: 
1. BibTeX 8-bit:
1. Biber:`"D:\LaTeX\MikTex\texmfs\install\miktex\bin\biber.exe" %`
1. Makeindex: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\makeindex.exe" %.idx`
1. Tixindy:
1. Makeglossaries:
1. Metapost: `"D:\LaTeX\MikTex\bin\mpost.exe" –interaction nonstopmode`
1. Asymptote: `"C:\Program Files\Asymptote\asy.exe" %.asy`
1. Ghostscript: `"C:\Program Files\gs\gs9.07\bin\gswin32c.exe"`
1. Latexmk: `"D:\LaTeX\MikTex\texmfs\install\miktex\bin\latexmk.exe" -e "$pdflatex=q\pdflatex -interaction=nonstopmode\" -pdf %.tex`

