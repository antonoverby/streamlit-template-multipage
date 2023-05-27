# Streamlit Template for Multipage Apps

Hello :wave:! This repo provides a template for the directories and files needed to begin a multipage streamlit app. Simply git clone the repository, rename to your app's name and add your own virtual environment.
***
## Folder Structure

```
|   .gitignore
|   main.py
|   README.md
|   requirements.txt
|
+---.streamlit
|       config.toml
|
+---app
|       utils.py
|
+---assets
+---data
\---pages

```
***
## Directory/File Descriptions

**.gitignore**: Directories and files that will not be committed to the git repository or GitHub

**main.py**: Displays the homepage of your app

**README.md**: You are here. Use it to describe your project.

**requirements.txt**: Where library dependencies will be recorded. Run the following in your command line to update once libraries are installed:

```bash
pip freeze > requirements.txt
```

**.streamlit/**: Holds config file

- **config.toml**: Configures various options that affect your app globally. For example, this config file is set to dark mode theme by default.

**app/**: Holds helper files for the app

* **utils.py**: Code that can be reused on multiple pages in the app. For example a function that sets a page header can written here, imported onto a page file and declared there instead of rewriting the code line-for-line on each page that needs the header.

**assets/**: Holds images files and other files that need to be accessed by pages

**data/**: Holds data

**pages/**: Holds each page as a separate file. Must be called "pages" in order for Streamlit to recognize it as a multipage app.

***


