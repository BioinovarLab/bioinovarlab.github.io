# Bioinovar LAB website

Content of the ...

## Update publications
Publications are managed with a Google scholar public profile. To update them on Jekyll you have to export the list to Bibtex format on your computer:

1. Log in to [Google Scholar](https://scholar.google.com) with IoT-LAB account
2. Click *My citations*
3. Click the leftmost checkbox (i.e. *Title*) on the bar at the top of the list of citations
4. Click *Export>BibTex>Export all my articles*
5. *Save as...* page in publications.bib file

Finally you have to generate the YAML file in the *_data* directory and commit it.

    sudo apt-get install pandoc-citeproc
    pandoc-citeproc -y publications.bib > _data/publications.yml
