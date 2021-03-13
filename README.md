Taken from:
http://dud.inf.tu-dresden.de/~ben/evince_synctex.tar.gz

See:
https://tex.stackexchange.com/questions/2941/how-to-setup-synctex-with-vim-pdflatex-and-an-open-source-pdf-viewer-under-linu


For vscode, the settings would be as follows:
```typescript
    "latex-workshop.view.pdf.viewer": "external",
    "latex-workshop.view.pdf.external.viewer.command": "evince",
    "latex-workshop.view.pdf.external.synctex.command": "evince_forward_search",
    "latex-workshop.view.pdf.external.synctex.args": [
        "%PDF%",
        "%LINE%",
        "%TEX%",
    ]
```
