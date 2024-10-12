# Typst template for two-column IEEE-like papers at the Cooperative State University Baden-Würrtemberg

This file aims to give a short overview of how IEEE-like papers can be created using this repo. For an introduction to the markup-based typesetting system *Typst*, please refer to the official [documentation](https://typst.app/docs/).

## Template
The paper is defined according to the `template.typ` file. For many use cases this file will not need changing.

## Thesis
Your thesis starts with the `thesis.typ` file. A document is created here based off `template.typ`.

## Content
Your content may be separated into separate files per chapter, which can be placed in the `/chapters` folders. These files must then be included into the `thesis.typ` file using the following command:

```Typst
#include "./chapters/introduction.typ"
```

## Literature
Place your literature into `literature.bib` in BibTex style.

## Acronyms
Place your acronyms into `acronyms.yaml` in the following style:

```YAML
YAML: YAML Ain't Markup Language
```

## Static file
Place static files like images into the `/statics` folder and include them in your thesis according to the documentation.

## Compilation
Compile your thesis using the Typst CLI.

To compile your thesis once, use the following command:

```SHELL
typst compile thesis.typ
```

To compile your thesis upon change, use the following command:
```SHELL
typst watch thesis.typ
```

That should be all :)
