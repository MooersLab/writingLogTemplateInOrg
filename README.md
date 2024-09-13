![Version](https://img.shields.io/static/v1?label=writingLogTemplateOrg&message=0.7.2&color=brightcolor)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)


# Writing log template in org-mode

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
- A GUIDANCE drawer that stores advice on how to use a section. The drawer is opened by placing the cursor on it and entering tab.


### Introduction

The writing log is a document that is external to the manuscript.
It stores the plans and progress made on one manuscript.
It is a tool for enhancing your focus and sustaining forward momentum on the writing project.
It is also a tool that eases re-engagement in an interrupted writing project.
It is like a master thinking document or a second brain for a writing project.

Instructions for using the writing log are found in the annotations in the template.
You can delete these after they are no longer needed.

Version 0.5 of the writing log is divided into four sections: 

- project initiation
- project data
- plans to support the project
- timely completion
- daily entries
- future additions and tangents
- Guidelines, checklists, protocols, and helpful tips

The subsections of these sections are shown below.

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

Create the following yasnippet snippet with the tab trigger of `daily` to autogenerate a subsection heading, property box, and index key using today's date.
Save it to a file named daily-entry-for-writing-log inside `./snippets/org-mode`.

```elisp
# -*- coding: utf-8 -*-
# group: writing-log
# name: daily-entry-for-writing-log
# key: daily
# --
** `(format-time-string "%Y-%m-%d")`
:PROPERTIES:
:CUSTOM_ID: `(format-time-string "%Y-%m-%d")`
:END:
#+Latex:\index{`(format-time-string "%Y-%m-%d")`}
$0
```

Now type `daily` followed by `tab` to start a new subsection for the current day's entry.


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

- Daily Protocol
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
  + `C-3 S-tab` to collapse the whole document while showing headlines down to the 3rd level. Change the number to collapse to a different level.
  + `C-x C-o` to show the outline view using consult. This is the same as `M-x consult-outline`. This consult command collapses the document into a more compact format than `C-s S-tab` command. It is easier to navigate as a result. You have to install the consult package.

The [latex-emacs profile](https://github.com/MooersLab/latex-emacs) can access org-mode because it is built into Emacs.

## Using with org-pomodoro

The daily log section is the ideal place for running a pomodoro timer.
The daily entries have a property drawer.
Place the cursor or point below the current day's heading and enter `C-c o` to start a pomodoro with the start and end times logged in a logbook in the property drawer.




## Bash function for creating writing log for new project

At the start of a writing project, use this function to write a copy of the writing log template to a file with the project name in it.
Store this Dash function in the `.bashrc` or `.zshrc` file. Oh shoot too

```bash
function logorg {
echo "Copy template writing log in org with project number in title."
if [ $# -lt 1 ]; then
  echo 1>&2 "$0: not enough arguments"
  echo "Usage1: logorg projectID"
  return 2
elif [ $# -gt 1 ]; then
  echo 1>&2 "$0: too many arguments"
  echo "Usage1: logorg projectID"
  return 2
fi
projectID="$1"
echo "Write writing log to log$1.org file."
cp  ~/6112MooersLabGitHubLabRepos/writingLogTemplateInOrg/writingLogTemplateVer5.org log$1.org
}
```


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
| Version 0.1 | First working version.                                                                     | 2022 September 10    |
| Version 0.5 | Added five sections to catch up with the tex version.                                      | 2024 August 11      |
| Version 0.6 | Compiles now without init.el file. Moved `Daily protocol` to `Guidelines` section. Elevated  `Daily Log` to section level. | 2024 August 18      |
| Version 0.7 | Moved the comments or advice prose into a GUIDANCE drawer in each section outside of the Guidelines section. | 2024 August 21      |
| Version 0.7.1 | Added subheading with noexport tag above each GUIDANCE drawer to prevent the export of their contents to the PDF.  Added the urlx package to linewrap long URLs. | 2024 August 27      |
| Version 0.7.2 | Added STARTUP command to open file with the drawers closed. | 2024 September 13 |

## Sources of funding

- NIH: R01 CA242845
- NIH: R01 AI088011
- NIH: P30 CA225520 (PI: R. Mannel)
- NIH: P20 GM103640 and P30 GM145423 (PI: A. West)

