# A Org-mode writing log template for thinking, planning, and monitoring progress on writing projects 

Use this writing log in parallel to the main writing project document to track your progress and record your plans.

[Org-mode](https://orgmode.org/) is a rich variant of markdown (see [cheatsheet](https://devhints.io/org-mode)) that can read LaTeX code.

Use the org-mode markdown code as normal and re-use the LaTeX code as templates for figures and tables with captions.


## Features

- 20 considerations for planning a manuscript.
- A table of contents that is automatically generated.
- An automatically generated index.
- Support for generating a refernces cited section.
- A writing log section for recording notes by each day's accomplishments.
- code to plot to wordcount by writing session to track your progress

## Usage

- `git clone` into the folder containing your current writing project.
- Load the writingLogTemplate.org into Emacs. 
- Essential keybindings active in org-mode:
  + `C-g` to abort current command.
  + `C-c C-x` to quit Emacs
  + `C-x C-s` to save the current document.
  + `C-c C-e l o` to export to pdflatex and bibtex and open the resulting PDF in default PDF viewer.
  + `C-x u` to undo the last change.

The [latex-emacs profile](https://github.com/MooersLab/latex-emacs) can access org-mode because it is built into Emacs.

See [related talk](https://github.com/MooersLab/BerlinEmacsAugust2022).

## Related projects of possible interest

- [Org-mode manuscript template](https://github.com/MooersLab/manuscriptInOrg)
- [LaTeX manuscript template](https://github.com/MooersLab/manuscriptInLaTeX)
- [Writing log template in LaTeX (compiles on Overleaf and in Emacs)](https://github.com/MooersLab/writingLogTemplate)
- [Slideshow template in LaTeX](https://github.com/MooersLab/slideshowTemplateLaTeX)
- [Annotated bibliography Template in LaTeX](https://github.com/MooersLab/annotatedBibliography)
- [Diary for 2022 in LaTeX](https://github.com/MooersLab/diary2022inLaTeX)
- [Diary for 2023 in LaTeX](https://github.com/MooersLab/diary2023inLaTeX)
- [latex-emacs profile](https://github.com/MooersLab/latex-emacs)
- [snippets for latex-mode in Emacs](https://github.com/MooersLab/snippet-latex-mode)
- [Quizzes about Emacs to improve recall of keybindings](https://github.com/MooersLab/qemacs)
- [Slides from talk about GhostText, Data Science Workshop, July 2022](https://github.com/MooersLab/DSW22ghosttext)
- [Video link to talk about GhostText, Data Science Workshop, July 2022](https://mediasite.ouhsc.edu/Mediasite/Channel/python/watch/4da0872f028c4255ae12935655e911321d)
