# Josephs Lab Manuscript Template

Author: Miles Roberts*

*I made this template by using the biorxiv preprint latex template and making modifications.

## How to use

Copy all of the files in this repo into overleaf and use the prompts in each `.tex` file as a guide. As a general overview:

`main.tex` contains the main text of the manuscript

`supplement.tex` contains supplementary figures, methods, etc.

`reviews.tex` is a template for writing responses to reviewer comments

`library.bib` contains all references in .bib format, which can be exported from most reference managers. I recommend syncing your overleaf with zotero or something similar.

`cover.tex` is a simple template for writing a cover letter.

`figures/` contains separate folders for main figures and supplementary figures

You can replace `Josephs_transparent.png` with your own lab logo if you wish.

## Tracked changes

Overleaf will typically track changes if you have the paid version, but it can be annoying to have all of the tracks on screen when you're writing. A good practice is to label your overleaf versions (undernearth history tab) for each major milestone. For example, label the version you submit to biorxiv as `biorxivV1` or something similar. If you have labeled your versions, then it's easy to download an old version of a `.tex` file and compare it to a revised version with `latexdiff` on the command line:

`latexdiff old.tex new.tex > diff.tex`

where `diff.tex` will be a tracked changes version of your document.

You can install `latexdiff` with conda or [use it on overleaf](https://www.overleaf.com/learn/latex/Articles/How_to_use_latexdiff_on_Overleaf)