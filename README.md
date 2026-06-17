![Version](https://img.shields.io/static/v1?label=writingLogTemplateOrg&message=0.8.7&color=brightcolor)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)


# Writing project log template in org-mode: A space for metacognition and storing metadata about one writing project

## Problem addressed

This template addresses the problem of cluttering the writing project document with notes about decisions made and plans for the work.
This template provides a safe place for notes that often get deleted or lost upon manuscript submission.
These notes serve as a valuable resource for addressing questions from reviewers and readers.
They are also a valuable source of ideas for future papers and grant applications.


## What is this? 

Use this template to store, in one document outside your writing project's main document (e.g., journal article, grant application, book chapter, book, lecture notes, seminar notes, talk notes, poster notes), the data and the thinking behind your writing project.
This document is meant to be specific to one project.
It helps you maintain a sharp focus on the project in front of you for a few hours while ignoring all other projects and worries.
Create a separate document for additional projects.

## How does it differ from the accountability tool of the same name?

This writing log is different from the writing accountability tool that is also called a writing log.
The accountability tool is where you record the time that you spent on each of your writing projects on a given day.
There is support in this document for tracking word count, but I find it kind of pointless because the word count plateaus pretty quickly.
It can be difficult to monitor the number of words added and deleted during editing sessions, which make up the majority of the time spent on a research article.
It's better to record the number of minutes spent on a particular writing project on a given day to track progress.


## How to use this tool?

Use this writing log in parallel to the main writing project document to support these workflows:

- project ideation and initiation (usually a 3-4 hour work session on day one)
- Data inventory (update as needed)
- Daily log to record decisions made, actions completed or attempted, and correspondence.
- Periodic project assessment against timeline with milestones (once a week, month, or quarter -- whatever is appropriate)
- Project completion and archiving (one to several days at manuscript submission or acceptance, or a bit of both)

## Why use this writing project log?

- Eases restarting a project that has been interrupted.
- Supports working on several projects concurrently.
- Addresses the fear of losing momentum.
- Abates the fear of forgetting where you left off.
- Supports the planning of related projects as you make progress on the current project. You will have a running start on the next writing project.

## What this is not?

- This is not an extended annotated bibliography to store your thoughts about the literature you read. You can find elsewhere on this site repositories that support the assembly of classical annotated bibliographies. You will also find repositories for templates for modern bibliographies that support multi-paragraph entries illustrated with figures, tables, code listings, equations, and URLs to relevant websites, including videos.
- 
- This is not an accountability tool where you record your minutes spent or words written per day across one or more writing projects. You can find several approaches to writing accountability on this website, along with the corresponding tools to support them. You can choose one approach that you think you can use daily. Do not try to use more than one approach at a time. You will exhaust yourself and give up. If you schedule your writing activities and show up at the appointed time, the need to track your progress will diminish as following the writing schedule becomes a deeply ingrained habit.


## What is org-mode

[Org-mode](https://orgmode.org/) is a rich variant of markdown (see [cheatsheet](https://devhints.io/org-mode)) that can read some LaTeX code directly.
The remaining LaTeX code can be used in a LaTeX code block.


## Features

- 20 considerations for planning a manuscript.
- A table of contents that is automatically generated and hyperlinked.
- An automatically generated index that is hyperlinked.
- Support for generating a references cited section from a BibTeX library.
- A writing log section for recording notes about each day's accomplishments.
- Plot of the word count by writing session to track your progress.
- Use org-clock and clock tables to track and summarize your effort.
- A GUIDANCE drawer that stores advice on how to use a section. The drawer is opened by placing the cursor on it and pressing Tab.
- Transcluded AIuse.org that can be updated in one file and imported into writing logs for all projects.
- A table of zettelkasten nodes being actively used in this project.

## Related videos

Sick of reading? Here is a 20-minute [video](https://www.bing.com/videos/riverview/relatedvideo?q=EmacsConf+Blaine+Mooers&mid=F191ED7C7665BAB53B30F191ED7C7665BAB53B30&churl=https%3a%2f%2fwww.youtube.com%2fchannel%2fUCwuyodzTl_KdEKNuJmeo99A&FORM=VIRE) about this project.

## Claude skill file to semiautomate daily entries

The zip file update-writing-log.zip contains a Claude skill in a folder.
It has a subfolder with a Python script.
This skill will review the changes you have committed during the day via Git and any unsaved changes in the currently open manuscript file.
It does not depend on chat history, so the changes you make to the manuscript do not have to have been made in Claude.

It will summarize these changes and insert them at the appropriate position inside the Daily Log section.
This tool is meant to ease the task of making a daily entry.
That task is already fairly small, but nonetheless, this makes it even easier to do.
If you did additional work outside the folder containing the writing project, then you will have to enter those accomplishments manually.

### Introduction

The writing log is a document that is external to the manuscript.
It stores the plans and progress for a single manuscript.
It is a tool to enhance your focus and sustain forward momentum on the writing project.
It is also a tool that eases re-engagement in an interrupted writing project.
It is like a master thinking document or a second brain for a writing project.

Instructions for using the writing log are provided in the template's annotations.
You can delete these after they are no longer needed.

Version 0.8 of the writing log is divided into these sections: 

- Project initiation
- Project data
- Plans to support the project
- Timely completion
- Zettelkasten nodes in use
- Daily entries
- Future additions and tangents
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

### AI use

The section is transcluded using the org-transclude package.
This enables editing of this section in a single file and its import into the writing logs for many projects.
The section is under rapid change due to the evolving nature of AI.
Read the tutorial tutorialOrgTransclusion.org.

The information in this file is global.
You can add another section for project-specific AI use.
You should document your local AI use in the daily log section below.

### Project Data

- Inventory of data on hand
- Inventory of the project's required external software
- Inventory of the project's software repositories
- Relevant videos
- Relevant blogs
- Relevant literature sources
- Relevant collections of PDFs
- Project's progress summary for the annual grant report
- Project's progress summary for the annual report to the college


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
- Data management, including backups and archives.
- Data sharing.
- The NIH PEDP.
- Advertising plan: posters, talks, seminars, YouTube videos, social media posts.


### Project management for timely completion 

- Checklist for manuscript completion.
- Timeline and Milestones.
- Periodic assessments of the current state of the manuscript.

### Nodes Used in Zettelkasten

This section contains a table of the nodes used in this project.
You update this table as you use new nodes.
You may want to list the most appropriate parent node.
The idea is to jump back into the Zettelkasten by looking up the appropriate node.
Folgezettels make such navigation faster and less error-prone than relying on searches.

I realize that this goes against the idea of needing to search through your Zettelkasten to become more familiar with it and to stumble across pairs of nodes to cross-link.
However, busy academics need to get on with finding where they left off.

The table was positioned just above the daily entries, so it's easy to find and use each day.

### Daily entries

Create the following yasnippet snippet with the tab trigger of `daily` to auto-generate a subsection heading, property box, and index key using today's date.
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

Now type `entry` followed by `tab` to start a new subsection for the current day's entry.


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

This part of the writing project log may require customization.
You may want to include project-specific protocols.
You may have already written down your own protocols that you want to include, or the space for such protocols may stimulate you to develop protocols for multi-step processes you must go through in your work.
Having those multi-step processes recorded in a protocol and readily accessible in this document increases the probability that the protocol will be followed and that you will save time by avoiding mistakes.

We have made a variant of this writing log where this section is modular.
The modularity eases the inclusion and exclusion of various protocols and guidelines so that you can customize this section of the writing log to be most relevant to the writing project at hand.
Search this website for repositories containing the words "modular" and "writing log".

Below is a list of protocols you can delete, supplement,  or expand upon.
 
- Daily Protocol
- Tips for using Overleaf
- Protocol for running Grammarly in Overleaf
- Guidelines for debugging the annotated bibliography
- Graphical Abstract
- Guidelines for benchmarks
- Guidelines for using the Writing Progress Notebook
- Guidelines for using a personal knowledge base
- Protocol for wrapping up the project and archiving data.

#### Standard Protocols

We store files containing established protocols in the home directory.
These files can be included in all writing-project log files.
This enables updating a single file and propagating the updates to all log files.
In an org file, you can use the org-mode `#+INCLUDE:` or the LaTeX `\include{}`.
These included files will only be injected into the log file upon export to PDF.

To inject the contents of the external file into an org-mode file so that you see the protocol in the org file, use the following function.
It includes the file path of the injected file and a timestamp of when the external file was injected.

```elisp
(defun org-insert-external-file (file-path)  
  "Insert the contents of an external file into the current org-mode file.  
Prompts for a file path via minibuffer and includes a timestamp in a comment."  
  (interactive "fFile to be inserted: ")  
  (let ((timestamp (format-time-string "%Y-%m-%d %H:%M:%S")))  
    (insert (format "#+BEGIN_COMMENT\n# File %s inserted on %s\n#+END_COMMENT\n\n" file-path timestamp))  
    (insert-file-contents file-path)  
    (goto-char (point-max))))  
  
(global-set-key (kbd "C-c S") 'org-insert-external-file)
```
Here is an example of the output.

```org-mode
** Protocol to generate a bib file with only cited references
#+BEGIN_COMMENT
# File ~/protocols-org/bibfileCitedOnly-writing-checklist.org inserted on 2024-12-06 04:16:21
#+END_COMMENT
- [ ] Run the following code to generate a bib file of the papers cited in a manuscript:
- [ ] bibtool --preserve.key.case=on -x main.aux > cited.bib
- [ ] main.tex is the manuscript file.
- [ ] Note that the *main.aux* file is hidden on Overleaf under the "Logs and outputs" pulldown menu.
- [ ] The first flag in the command will preserve the letter case in the cite key.
```

Here is a modified form of the above function that prepends the file path to the protocols directory:

```elisp
(defun org-insert-protocol-file (file-path)  
  "Insert the contents of a protocol file from ~/protocols-org into the current org-mode file.  
Prompts for a file path via minibuffer and includes a timestamp in a comment."  
  (interactive (list (read-file-name "Directory `~/protocols-org/`: " "~/" "protocols-org/")))  
  (let ((full-path (expand-file-name file-path))  
        (timestamp (format-time-string "%Y-%m-%d %H:%M:%S")))  
    (insert (format "#+BEGIN_COMMENT\n# File %s inserted on %s\n#+END_COMMENT\n\n" full-path timestamp))  
    (insert-file-contents full-path)  
    (goto-char (point-max))))  
  
(global-set-key (kbd "C-c P") 'org-insert-protocol-file)
```

Disclosure: The last two functions were generated with Lama 3.1 70B via the Sider plugin for Google Chrome.
The functions were tested, and they worked as advertised.

## Usage

- `git clone https://github.com/MooersLab/writingLogTemplateInOrg` into the folder containing your current writing project.
- Start Emacs, perhaps using this [Emacs configuration](https://github.com/MooersLab/dsw-2024-org-mode-init).
- Load the writingLogTemplate.org file into Emacs via `C-x C-f`. 

## Configure yasnippets

You may want to enable yasnippets to make your LaTeX and org-mode snippets available while editing the writinglog.org file in org-mode.

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
  + `M-UP` or `M-DOWN` to shift lines up and down. UP and DOWN are the arrow keys.
  + `C-3 S-tab` to collapse the whole document while showing headlines down to the 3rd level. Change the number to collapse to a different level.
  + `C-x C-o` to show the outline view using consult. This is the same as `M-x consult-outline`. This consult command collapses the document into a more compact format than `C-s S-tab` command. As a result, it is easier to navigate. You have to install the consult package.

The [latex-emacs profile](https://github.com/MooersLab/latex-emacs) can access org-mode because it is built into Emacs.

## Using with org-pomodoro

The daily log section is the ideal place for running a Pomodoro timer.
The daily entries have a property drawer.
Place the cursor or point below the current day's heading and enter `C-c o` to start a Pomodoro with the start and end times logged in a logbook in the property drawer.


## Bash function for creating a writing log for a new project

At the start of a writing project, use this function to write a copy of the writing log template to a file with the project name.
Store this Bash function in the `.bashrc` or `.zshrc` file or wherever you store your aliases. 

```bash
function logorg {
echo "Copy template writing log in org with project number in title."
if [ $# -lt 1 ]; then
  echo 1>&2 "$0: Not enough arguments."
  echo "Usage1: logorg projectID"
  return 2
elif [ $# -gt 1 ]; then
  echo 1>&2 "$0: Too many arguments."
  echo "Usage1: logorg projectID"
  return 2
fi
projectID="$1"
echo "Write writing log to log$1.org file."
cp  ~/6112MooersLabGitHubLabRepos/writingLogTemplateInOrg/writingLogTemplateVer087.org log$1.org
}
```

## Some relevant functions in [Mooerslab/mooereslab-functions-el](https://github.com/MooersLab/mooerslab-functions-el)

This repository contains my collection of useful functions to ease the use of this writing log and org-mode in general.

- add-periods-to-list
- org-add-periods-to-list-items
- org-insert-protocol-file (I now store my protocols in ~/org-roam for fast discovery and recall)
- region-to-itemized-list-in-org
- region-to-todos-in-org
- region-to-itemized-in-latex
- latex-to-org-list-region
- region-csv-to-org-table
- create-org-table-with-caption
- count-non-blank-lines
- export-csv-to-sqlite-table (great for creating databases from CSV files)
- export-csv-to-matched-sqlite-table (great for adding data in a CSV file to an existing database)
- get-citekeys-from-bibtex-file
- wrap-citekey-and-create-tex-file
- insert-org-captioned-figure 
- org-convert-checkboxes-to-todos
- org-move-to-tag
- append-todo-to-tagged-headline
- open-new-abibnote-on-citekey
- split-sentences-into-lines (very useful for splitting the long line of sentences returned from the whisper-file transcription)

## Directly related talks
- [DSW 60-minute talk about scientific writing workflow in Org Mode: November 22, 2024](https://mediasite.ouhsc.edu/Mediasite/Channel/python/watch/cd5641aea892468c894ae31cd151d4671d)
- [Slides from the above talk](https://github.com/MooersLab/DSW24-org-mode-slides)
- [Emacs configuration associated with the above talk](https://github.com/MooersLab/dsw-2024-org-mode-init)

- [EmacsConf24 20-minute talk: December 7, 2024](https://emacsconf.org/2024/talks/project/)

## Related projects of possible interest
- [Org-mode manuscript template](https://github.com/MooersLab/manuscriptInOrg)
- [LaTeX manuscript template](https://github.com/MooersLab/manuscriptInLaTeX)
- [Writing log template in LaTeX (compiles on Overleaf and in Emacs)](https://github.com/MooersLab/writingLogTemplate)
- [Writing log template in reStructuredText](https://github.com/MooersLab/writing-log-rst) reStructuredText is used by programmers for documentation.
- [Writing log template in Markdown](https://github.com/MooersLab/writing-log-md) Markdown variant. Read and rendered to PDF by most good text editors.
- [Writing log template in ODT](https://github.com/MooersLab/writing-log-odt) ODT can be read by Open Office, LibreOffice, and MS Word.
- [Writing log template in DOCX for MS Word](https://github.com/MooersLab/writing-log-docx) MS Word variant. Probably the least suitable format for this task.
- [Programming log in Org](https://github.com/MooersLab/programmingLogInOrg)

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
|  0.1 | First working version.                                                                              | 2022 September 10    |
|  0.5 | Added five sections to catch up with the tex version.                                               | 2024 August 11      |
|  0.6 | Compiles now without init.el file. Moved `Daily protocol` to `Guidelines` section. Elevated  `Daily Log` to section level. | 2024 August 18      |
|  0.7 | Moved the comments or advice prose into a GUIDANCE drawer in each section outside of the Guidelines section. | 2024 August 21      |
|  0.7.1 | Added subheading with noexport tag above each GUIDANCE drawer to prevent the export of their contents to the PDF.  Added the urlx package to linewrap long URLs. | 2024 August 27      |
|  0.7.2 | Added STARTUP command to open file with the drawers closed. | 2024 September 13 |
|  0.7.3 | Explained introduction to distinguish this tool from writing accountability tools. | 2024 October 30 |
|  0.8.0 | Added :restart: tag to position the cursor at the end of the last daily entry in the Daily Log section upon opening the document in Emacs. Made minor updates to the README.md file, including a link to talk about this document. | 2024 November 28 |
| 0.8.1 | Added function to insert contents of external files. This is very cool!                            | 2024 December 6 |
| 0.8.2 | Added :appendtodos: tag to headline above TODO list in the middle of the document to work with org-projects.el. Replaced Next Action with  Hemingway Bridge.                           | 2025 March 21 |
| 0.8.3  | Added list of useful functions found in mooerslab-functions-el                         | 2025 March 27 |
| 0.8.4 | Added section at the beginning for drafting alternate central hypotheses.  | 2026 January 5|
| 0.8.6 | Added transcluded section on AI use. | 2026 April 17|
| 0.8.7 | Added section just above daily log for table of nodes used in zettelkasten. | 2026 May 24 |

## Sources of funding

- NIH: R01 CA242845
- NIH: R01 AI088011
- NIH: P30 CA225520 (PI: R. Mannel)
- NIH: P20 GM103640 and P30 GM145423 (PI: A. West)


<!-- Local Variables: -->
<!-- jinx-local-words: "BibTeX" -->
<!-- End: -->
