# A Org-mode writing log template 

Use this writing log in parallel to the main writing project document to track your progress and record your plans.

[Org-mode](https://orgmode.org/) is a rich variant of markdown (see [cheatsheet](https://devhints.io/org-mode)) that can read LaTeX code.

Use the org-mode markdown code as normal and re-use the LaTeX code as templates for figures and tables with captions.


## Features

- 20 considerations for planning a manuscript.
- A table of contents that is automatically generated and hyperlinked.
- An automatically generated index that is hyperlinked.
- Support for generating a references cited section form a Bibtex library.
- A writing log section for recording notes by each day's accomplishments.
- Plot of wordcount by writing session to track your progress.

## Usage

- `git clone https://github.com/MooersLab/writingLogTemplateInOrg` into the folder containing your current writing project.
- Start Emacs, perhaps using the [latex-emacs](https://github.com/MooersLab/latex-emacs) profile.
- Load the writingLogTemplate.org file into Emacs via `C-x C-f`. 

## Configure yasnippets

You may want to enable yasnippets to make available your latex-mode and org-mode snippets while editing the writinglog.org file in org-mode.

1. In your `~/.emacs.d/snippets/latex-mode`, create a file named `.yas-parents`.
2. Add the following to this file:

```elisp
latex-mode
org-mode
```
3. Under the Yasnippets pulldown, select `reload everything` or in the minibuffer, enter `M-x yas-reload-all`.
 

## Essential keybindings for editing this file in in org-mode:
  + `C-g` to abort current command.
  + `C-x C-c` to quit Emacs
  + `C-x C-s` to save the current document.
  + `C-c C-e l o` to export to pdflatex and bibtex and open the resulting PDF in default PDF viewer.
  + `C-x u` to undo the last change.
  + `M-UP` or `M-DOWN` to shift lines up and down. UP and Down are the arrow keys.

The [latex-emacs profile](https://github.com/MooersLab/latex-emacs) can access org-mode because it is built into Emacs.

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
- [Slides to talk given August 31, 2022](https://github.com/MooersLab/BerlinEmacsAugust2022)
- [Slides from talk about GhostText, Data Science Workshop, July 2022](https://github.com/MooersLab/DSW22ghosttext)
- [Video link to talk about GhostText, Data Science Workshop, July 2022](https://mediasite.ouhsc.edu/Mediasite/Channel/python/watch/4da0872f028c4255ae12935655e911321d)
- [The writer's law](https://github.com/MooersLab/thewriterslaw)
