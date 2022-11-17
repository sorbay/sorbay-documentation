# Sorbay Documentation

The documentation is based on MkDocs resp. Material for MkDocs as theme.

https://squidfunk.github.io/mkdocs-material/
https://www.mkdocs.org/


## Installation required development tools

You need python 3.x installed and pip package manager!

Install older version of Markdown package, as the latest one is not compatible with the defined versions of the mkdocs dependency:
`pip install Markdown==3.3.7`

Install other dependency for mkdocs-material:
`pip install mkdocs-material`

You might want to add the installation folder to your path variable so you can execute the commands without defining the file location path.
Add `export PATH=$PATH:$HOME/.local/bin` to your `.bashrc` file.

## Live development

To preview the documentation site run: `mkdocs serve`  
To change the port you can use the `-a` option: `mkdocs serve -a localhost:8088`  
Open the browser and you will see the documentation site. Chaning any page will automatically refresh the view.

## Github Pages deployment

* Switch into branch containing the version you want to deploy
* Run `$ mkdocs gh-deploy`
* Check status of Github deployment action: https://github.com/sorbay/sorbay-documentation/actions
* Once finished, check the documentation: https://doc.sorbay.com/