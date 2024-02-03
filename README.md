# nsf_coa_table4
Repo to generate an updated Table 4 for an NSF Collaborators and Other Affiliations document<br>
Written by M. Siegfried, 29 Jan. 2023<br>
siegfried@mines.edu

The notebook `make_coa_table4.ipynb` updates Table 4 of the NSF's Collaborators and Other Affiliations (COA) document based on a bibtex file (`.bib`) that contains only publications you were a part of and does this update in way that you can then just copy and paste the contents into your COA (download the NSF COA template [here](https://www.nsf.gov/bfa/dias/policy/coa/coa_template.xlsx)). Easy peasy! Because it focuses on "updates", the first time you use it will take a bit of data cleaning, both in your bib file (e.g., "Matthew R. Siegfried, Matthew Siegfried, and M. R. Siegfried will become three different entries in your table until you clean the `.bib` file) and your Table 4 affiliations (in that you need to put them all in). If you have an old COA, you can copy and paste Table 4 into a temporary spreadsheet to use for initial merging of name-affiliations and then you'll be off to the races. Check the comments in the the notebook for more details on formatting, etc.

## Planned updates:
  * Handle latex accents in `.bib` file
  * Check for correct column header names and interactively prompt user to select appropriate headers
  * Make `pip` installable for power users

## Install and running
1. Clone repo into the folder you want `git clone https://github.com/mrsiegfried/nsf_coa_table4.git`
2. Install environment: `conda env create -f environment.yml`
3. Activate environment: `conda activate coa`
4. Install kernel into JupyterLab: `python -m ipykernel install --user --name coa`
5. Launch JupyterLab (`jupyter lab`) and run the cells




