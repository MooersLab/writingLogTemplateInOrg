![Version](https://img.shields.io/static/v1?label=writingLogTemplateOrg&message=0.5&color=brightcolor)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)


# Writing log for org-mode

Use this writing log in parallel to the main writing project document to track your progress and record your plans.

[Org-mode](https://orgmode.org/) is a rich variant of markdown (see [cheatsheet](https://devhints.io/org-mode)) that can read some LaTeX code directly.
The remaining LaTeX code can be used in a code block for LaTeX.

Use the org-mode markdown code as normal and reuse the LaTeX code as templates for figures and tables with captions.


## Features

- 20 considerations for planning a manuscript.
- A table of contents that is automatically generated and hyperlinked.
- An automatically generated index that is hyperlinked.
- Support for generating a references cited section from a Bibtex library.
- A writing log section for recording notes about each day's accomplishments.
- Plot of wordcount by writing session to track your progress.
- Use org-clock and clock tables to track and summarize your effort.


### Introduction

The writing log is a document that is external to the manuscript.
It stores the plans and progress made on one manuscript.
It is a tool for enhancing your focus and sustaining forward momentum on the writing project.
It is also a tool that eases re-engagement in an interrupted writing project.
It is like a master thinking document or a second brain for a writing project.

Instructions for using the writing log are found in the annotations in the template.
You can delete these after they are no longer needed.

Version 0.3 of the writing log is divided into four sections: 

- project initiation
- daily entries
- future additions and tangents
- Guidelines, checklists, protocols, and helpful tips

The subsections of these four sections are shown below.

### Project initiation

- Rationale
- Audience
- Target journals
- Related projects
- Potential Introduction
- Potential Results
- Potential Discussion points
- Prior discussion points
- Potential titles
- Potential keywords
- Potential abstract
- Abbreviations
- Potential collaborators
- Potential competitors
- Potential reviewers
- Draft cover letter

### Project Data

- Inventory of data on hand
- Inventory of project's required external software
- Inventory of project's software repositories
- Relevant videos
- Relevant blogs
- Relevant literature sources
- Relevant collections of PDFs
- Project's progress summary for annual grant report
- Project's progress summary for annual report to college



### Plans to support the project

- Budget
- Relation to specific aims of funded grants.
- Secure funding for the research and manuscript.
- Timeline to do the required experiments to test the hypothesis. 
- Secure access to required national laboratory resources at experimental stations (i.e., general user proposal and beamtime requests).
- Secure access to computing resources.
- Gather the appropriate information from the literature.
- Recruit collaborators
- Recruit lab members to do the work.
- Individual career development for lab members, including yourself.
- Biosafety.
- Authentication of key biological and chemical resources.
- Rigorous statistical sampling and data analysis
- Data management including backups and archives.
- Data sharing.
- The NIH PEDP.
- Advertising plan: posters, talks, seminars, YouTube videos, social media posts.


### Project management for timely completion 

- Checklist for manuscript completion.
- Timeline and Milestones.
- Periodic assessments of the current state of the manuscript.


### Daily entries

- Daily Protocol
- Daily Log
- Update writing progress notebook
- Update personal knowledge base
- Timeline or Benchmarks
- Next action
- To be done
- Word Count

### Future additions and tangents

- Ideas to consider adding to the manuscript
  + Introduction
  + Results
  + Discussion
- To be done someday
- Spin-off writing projects


### Guidelines, checklists, protocols, helpful hints
 
- Tips for using Overleaf
- Protocol for running Grammarly in Overleaf
- Guidelines for debugging the annotated bibliography
- Graphical Abstract
- Guidelines for benchmarks
- Guidelines for using the Writing Progress Notebook
- Guidelines for using a personal knowledge base

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
 

## Essential keybindings for editing this file in org-mode:
  + `C-g` to abort current command.
  + `C-x C-c` to quit Emacs
  + `C-x C-s` to save the current document.
  + `C-c C-e l o` to export to pdflatex and BibTeX and open the resulting PDF in the default PDF viewer.
  + `C-x u` to undo the last change.
  + `M-UP` or `M-DOWN` to shift lines up and down. UP and Down are the arrow keys.

The [latex-emacs profile](https://github.com/MooersLab/latex-emacs) can access org-mode because it is built into Emacs.

## Related projects of possible interest

- [Org-mode manuscript template](https://github.com/MooersLab/manuscriptInOrg)
- [LaTeX manuscript template](https://github.com/MooersLab/manuscriptInLaTeX)
- [Writing log template in LaTeX (compiles on Overleaf and in Emacs)](https://github.com/MooersLab/writingLogTemplate)
- [Writing log template in reStructuredText](https://github.com/MooersLab/writing-log-rst) reStructuredText is used by programmers for documentation.
- [Writing log template in Markdown](https://github.com/MooersLab/writing-log-md) Markdown variant. Read and rendered to PDF by most good text editors.
- [Writing log template in ODT](https://github.com/MooersLab/writing-log-odt) ODT can be read by Open Office, LibreOffice and MS Word.
- [Writing log template in DOCX for MS Word](https://github.com/MooersLab/writing-log-docx) MS Word variant. Probably the least suitable format for this task.
- [Slideshow template in LaTeX](https://github.com/MooersLab/slideshowTemplateLaTeX)
- [Annotated bibliography Template in LaTeX](https://github.com/MooersLab/annotatedBibliography)
- [LaTeX manuscript template](https://github.com/MooersLab/manuscriptInLaTeX/edit/main/README.md)
- [Org-mode manuscript template](https://github.com/MooersLab/manuscriptInOrg/edit/main/README.md)
- [Slideshow template in LaTeX](https://github.com/MooersLab/slideshowTemplateLaTeX)
- [Annotated bibliography Template in LaTeX](https://github.com/MooersLab/annotatedBibliography)
- [Diary for 2024 in LaTeX](https://github.com/MooersLab/diary2024inLaTeX)- [latex-emacs profile](https://github.com/MooersLab/latex-emacs)
- [default Emacs profile](https://github.com/MooersLab/configorg)
- [snippets for latex-mode in Emacs](https://github.com/MooersLab/snippet-latex-mode)
- [Quizzes about Emacs to improve recall of keybindings](https://github.com/MooersLab/qemacs)
- [Slides from talk about GhostText, Data Science Workshop, July 2022](https://github.com/MooersLab/DSW22ghosttext)
- [Video link to talk about GhostText, Data Science Workshop, July 2022](https://mediasite.ouhsc.edu/Mediasite/Channel/python/watch/4da0872f028c4255ae12935655e911321d)
- [Slideshow about using LaTeX in Emacs, Berlin Emacs Meetup, 31 August 2022](https://github.com/MooersLab/BerlinEmacsAugust2022)
- [The writer's crede](https://github.com/MooersLab/thewriterslaw)


## Update history

|Version      | Changes                                                                                      | Date                 |
|:-----------|-----------------------------------------------------------------------------------------------|:--------------------|
| Version 0.5 |   Added five sections to catch up with the tex version.                                      | 2024 August 11      |



## Sources of funding

- NIH: R01 CA242845
- NIH: R01 AI088011
- NIH: P30 CA225520 (PI: R. Mannel)
- NIH: P20 GM103640 and P30 GM145423 (PI: A. West)

