## rylan-thesis-template
This template is based on Rylan Shearn's PhD thesis and follows the requirements for theses that are to be submitted to Edith Cowan University - Faculty of Health, Engineering and Science for the award of a PhD/Masters/Honours. To view the full finished product of the thesis, see [here](http://ro.ecu.edu.au/theses_ebooks/1/). This template has been made publicly available after having a number of requests for the code. If you use it for your thesis or other type of book, it would be appreciated if you acknowledge the work somewhere in the text.

## Requirements
For the document to compile properly you need to:
- have latex installed
- have biblatex installed
- have biber installed
- make sure you are compiling with biblatex using the biber backend (ie. not using bibtex)

The safest option is to make sure you have the same setup as the test system (see installation instructions below).

## Installation instructions
### Linux
If you are running Ubuntu or similar, 

- open a terminal with `ctrl+alt+t` and enter the following:

```sh
sudo apt-get install texlive
sudo apt-get install texlive-latex-extra
sudo apt-get install texlive-bibtex-extra biber #needed for biblatex to run with biber
sudo apt-get install texlive-science # needed for some math packages
sudo apt-get install texstudio # tex editor
```
- Hit `enter` and `yes` to installation questions

- After installation, open TexStudio, make sure that BibLaTeX is selected by going to the `Bibliography` menu, then at the bottom there should be `Type:BibTeX` or `Type:BibLaTeX`, make sure it is `BibLaTeX`

- In TexStudio, select `options` menu, then `configure TeXstudio` then on the left, click on `Build` and make sure `Default Bibliography Tool` is set to `Biber`

### Other operating systems
You should be able to install the same packages for Windows and Mac, just google the installation instructions. I haven't tested anything on these operating systems but it should work.

## Usage
Download the `.zip` file, then extract anywhere you like.

### File layout
The file `main.tex` 
- loads required packages
- controls most of the document formatting (including reference formatting)
- contains the front matter text of the manuscript (title page, abstract etc)
- pulls in the content of each chapter from separate `.tex` files that are located in `/chapters`. So to add new chapters, you need to create a new `.tex` file in the `/chapters` directory, then edit `main.tex` in order to have it pulled into the document at a position of your choice.

The file `/chapters/introduction.tex` contains example formatting of:
- inserting and cross referencing figures
- inserting and cross referencing information boxes
- inserting and cross referencing tables
- inserting and cross referencing footnotes
- inserting and cross referencing biblatex bibliography entries
- inserting 'fancy' quotes

The file `main.bib` contains biblatex entries that can be called from within chapters or `main.tex`. You will need to add your own references to this file in the correct format.

### Compiling the document
To compile, use TexStudio, and make sure you have followed the installation instructions and the required settings for TexStudio above, then open `main.tex` in TexStudio and:

- click on the `Build and View` button or `F1`
- click `tools` then `bibliography` or `F11`
- click on the `Build and View` button or `F1` a second time

You should then have the PDF compiled correctly in the same directory
