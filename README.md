# MeiTing Trunk
An open source reference management tool developed in PyQt5 and Python3.

## Features

### Libraries

* Create, manage and switch between multiple libraries.

### Folders

* Oragnize documents in a folder tree, with arbitrary level of folder nesting.
* Add a document to multiple folders without taking up duplicate storage.

### Import format

* Import via bibtex files.
* Import via RIS files.
* Import PDF files (currently with limited meta data fetching capability).
* Update meta data using DOI.

### Export format

* Export to bibtex.
* Export to RIS.
* Bulk export, per folder, or per document.

### Searching and filtering

* Filter document using authors, keywords, tags or publications.
* Search meta data within folders or library.
* Duplicate checking within folders or library.

### Note taking

* Jot down your thoughts while reading, in your referred editor. (currently with limited formating options).

### Database

* Meta data saved in sqlite format, transparent and easy to manipulate.
* library saved in a portable manner, backup or share using your prefered online/offline tools.

### Full text search (experimental)

* Utilises Xapian engine to enable full text search inside attachment files (including PDFs, docs etc.).


### PDF preview and reader

* Use `pdf.js` as a build-in PDF reader.
* Use `poppler` to generate PDF thumbnails.


### Free and open source

* Open to suggestions, bug reports and new ideas.


## Screenshots

Main interface

![](https://user-images.githubusercontent.com/8076931/55284312-b651c700-53a6-11e9-9478-cb6ab8e89cf3.png)

Bulk export.

![](https://user-images.githubusercontent.com/8076931/55284318-d5e8ef80-53a6-11e9-9db9-560082253c2e.png)

Duplicate checking results.

![](https://user-images.githubusercontent.com/8076931/55284321-e4cfa200-53a6-11e9-8b6f-9e686d339acc.png)

Merge duplicates.

![](https://user-images.githubusercontent.com/8076931/55678909-5aea8080-5934-11e9-87bf-575fb99e3697.png)

Meta data searching.

![](https://user-images.githubusercontent.com/8076931/55284338-324c0f00-53a7-11e9-97a1-cd0e197ec012.png)

Full text search.

![](https://user-images.githubusercontent.com/8076931/56464555-f42e9200-641e-11e9-96b5-b57889ea11fa.png)

Actions on documents.

![](https://user-images.githubusercontent.com/8076931/55284334-23fdf300-53a7-11e9-9e34-01a1ae514a72.png)

Merge inconsistent journal names

![](https://user-images.githubusercontent.com/8076931/56706874-299ded00-6749-11e9-96ee-d59f76f874e2.png)


## Platforms and Dependencies

Currently only support Linux and MacOS.

### Python dependencies

* python3+
* PyQt5>=5.12
* PyQtWebEngine (this is no longer shipped with PyQt5 after 5.11)
* sqlite3
* pdfminer.six
* PyPDF2
* beautifulsoup4
* bibtexparser
* fuzzywuzzy
* crossrefapi
* RISparser
* send2trash
* python-levenshtein (optional)


### Other dependencies

* xapian-core, xapian-omega and the python bindings of xapian (all optional), required for full text searching. See https://xapian.org/docs/install.html for installation instructions. Also checkout the [wiki page](https://github.com/Xunius/MeiTingTrunk/wiki/Enable-snippets-in-full-text-search-results) on how to enable snippets.

* [poppler](https://poppler.freedesktop.org/) (optional), used for generating PDF thumbnails.


## Install

## install using pip


```
pip install meitingtrunk
```

Then launch it in the terminal with


```
$ meitingtrunk
```

To upgrade:


```
pip install --upgrade meitingtrunk
```


## Manual install

You can clone this repo

```
git clone https://github.com/Xunius/MeiTingTrunk
```

Check out the dependency list if any module is missing in your python environment.

Then launch it with

```
$ cd MeiTingTrunk
$ python -m MeiTingTrunk.main
```



## Contribution

This software is still in its very early stage. Please consider helping by trying it out, sending issues, suggestions, ideas or contributing code.

Major features that are still lacking (I greatly appreciate any help with any of them):

* Format citations into various citation styles, in a format suitable to paste into word editors.
* Import from Zotero.
* Other document types aside articles and books.
* Packaging into a format suitable for a few mainstream Linux package management tools.
* Of cource, any stability or performance improvements.



## Licence

This file is distributed under the terms of the
GPLv3 licence. See the LICENSE file for details.
You may use, distribute and modify this code under the
terms of the GPLv3 license.
