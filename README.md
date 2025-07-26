# Josephs Lab Manuscript Template

Author: Miles Roberts*

*I made this template by using the biorxiv preprint latex template and making modifications.

## How to use

Copy all of the files in this repo into overleaf and use the prompts in each `.tex` file as a guide. As a general overview:

`main.tex` contains the main text of the manuscript

`supplement.tex` contains supplementary materials, etc.

`reviews.tex` is a template for writing responses to reviewer comments.

`library.bib` contains all references in .bib format, which can be exported from most reference managers. I recommend syncing your overleaf with zotero or something similar.

`cover.tex` is a simple template for writing a cover letter.

`figures/` contains separate folders for main figures and supplementary figures

You can replace `Josephs_transparent.png` with your own lab logo if you wish.

## Labeling figures

Give your figures a unique label with `\label{WHATEVER}`. This project uses the xr package so that even the supplemental figures you add to supplement.tex can be referenced with their appropriate labels in main.tex

## Tracked changes

Overleaf will track changes in your .tex file if you have the paid version, but it can be annoying to have all of the tracks on screen when you're writing and these tracks won't render into a pdf that you can then turn into a journal or peer reviewer. You can generate a tracked changes pdf though by comparing a new .tex file to its older version.

**Tip**: A good practice is to label your overleaf versions (undernearth history tab) for each major milestone. For example, label the version you submit to biorxiv as `biorxivV1` or something similar. If you have labeled your versions, then it's easy to download the proper old version of a `.tex` file and compare it to a revised version.

### latexdiff on command line

Install `latexdiff` on the command line and get the two tex files you want compare:

`latexdiff old.tex new.tex > diff.tex`

### latexdiff on overleaf

Or you can just use latexdiff on overleaf. Download an old version of your main.tex file by going through your version history (hopefully you labeled your versions!) and then add it to your project as old.tex. Then compile the diff.tex file in your project.

This solution comes from the [overleaf documentation](https://www.overleaf.com/learn/latex/Articles/How_to_use_latexdiff_on_Overleaf)