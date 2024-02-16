# GVSU Introductory Physics Lecture Notes

## Overview

These directories will contain *markdown versions* of [my pdf handwritten lecture notes for each of these courses](https://drive.google.com/drive/folders/1xTeJMP0qe1BAhTBepOhjJ5PRLVJRBaHC?usp=share_link) (see also my associated *lecture videos* for [PHY220](https://www.youtube.com/watch?v=-oNpcZg7i8E&list=PLjSlnDpzlUokf0G9DC6LxAFRRfG-LxrBZ), some topics in [PHY231/234](https://www.youtube.com/watch?v=uI8p4nRM9k8&list=PLjSlnDpzlUomCQqfgN1mrYYZU7VLhL_OZ&pp=iAQB), and a few for [PHY221](https://www.youtube.com/watch?v=uI8p4nRM9k8&list=PLjSlnDpzlUokhoQcIyhVVS-PVht7r14xa&pp=iAQB)).

This is a work in progress: so far only a few of the PHY 231/234 notes are available as markdown text.  The directories will be updated over time.

## Workflow for markdown file creation

1. Copy pdf version of lecture notes to a directory
2. Extract one page as a png file
```
> pdftk 06_equipotential-capacitance.pdf cat 1 output junk.pdf && convert -density 200 junk.pdf junk.png
```
3. Open a new ChatGPT chat instance and use the following prompt with the attached `junk.png` file:
```
Please transcribe the text from the uploaded image into plain text, including LaTeX for the mathematical content. The equations should be formatted as raw LaTeX code, suitable for copying and pasting directly into a Markdown or LaTeX document. Place it in a "markdown" style code window for copying.

Inline math should be enclosed in single dollar signs, like this: $X$.

Block equations should be on separate lines with \\[ and \\] delimiters, like this:

\[
y = mx + b
\]

Please do not compile the LaTeX into display mode, I need the raw code for editing purposes.
```
4. Copy the junk.png file into the `images` directory.  Make multiple copies of it, one for each figure appearing on that page.  Give images names like `06_capacitor-w-dielectric.png`
5. Open each image png file in Preview and crop (cmd-k) the figure.
5. Copy the ChatGPT transcript into a markdown file (`06_equipotential-capacitance.md`) and adjust things:
    - Adjust headings how you want
    - make block equations by replacing the ChatGPT `\[` with \`\`\`math and `\]` with \`\`\`.
    - Check for ChatGPT hallucinations (it will change equations if it doesn't like them, or thinks they would be better based on the rest of the text).
6. Insert figures into text using, e.g.,
```
![Inserting a dielectric into a capacitor reduces the electric field (if that capacitor has been charged and disconnected from the battery beforehand)](images/06_capacitor-w-dielectric.png)
```
7. `git add` all files (markdown and images), commit, and push to github.
8. Repeat for next page.

## Fix-me's (2024)

* Fix indentation alignment for paragraphs and other elements (images, equation blocks) within itemized/enumerated lists.  It seems that this can be done cleanly for a sequence of paragraphs and inserted images, but adding a (math) code block breaks it.

* center figures with html "align"?






