# rylan-thesis-template
Rylan Shearn's PhD thesis template (based Edith Cowan University format requirements)

# tested with
texstudio

# Requirements
For the document to compile properly you need to:
- have latex installed
- have biblatex installed
- have biber installed
- make sure you are compiling with biblatex using the biber backend (ie. not using bibtex)

The safest option is to make sure you have the same setup as the test system (see installation instructions below).

# Installation instructions
## Linux
If you are running Ubuntu or similar, 
1. open a terminal with `ctrl+alt+t` and enter the following:

```
sudo apt-get install texlive
sudo apt-get install texlive-latex-extra
sudo apt-get install texlive-bibtex-extra biber #needed for biblatex to run with biber
sudo apt-get install texlive-science # needed for some math packages
sudo apt-get install texstudio # tex editor
```
2. Hit `enter` and `yes` to installation questions

3. After installation, open TexStudio, make sure that BibLaTeX is selected by going to the `Bibliography` menu, then at the bottom there should be `Type:BibTeX` or `Type:BibLaTeX`, make sure it is `BibLaTeX`

4. In TexStudio, select `options` menu, then `configure TeXstudio` then on the left, click on `Build` and make sure `Default Bibliography Tool` is set to `Biber`

## other operating systems
You should be able to install the same packages for Windows and Mac, just google the installation instructions. I haven't tested anything on these operating systems but it should work.


