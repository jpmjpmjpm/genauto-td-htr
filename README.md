[![CC BY 4.0][cc-by-shield]][cc-by]
![Lines Badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/jpmjpmjpm/f9d911269b14e279fca33a4224279234/raw/lines.json)
![Chars Badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/jpmjpmjpm/f9d911269b14e279fca33a4224279234/raw/chars.json)
![Region Badges](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/jpmjpmjpm/f9d911269b14e279fca33a4224279234/raw/regions.json)

# GenAuto TD Corpus

## Description

Ground Truth dataset for French handwritten pages of Civil Registry "Tables Décennales"

## Content

**150 images and Alto XML files divided into 3 sub-corpus.**

**Only first names, last names and dates are transcribed and only for birth sections of the documents.**

The Alto files contain:

- Segmentation of the transcribed texts.
- Transcription of the texts.
- Polygonalization of the transcribed text zones (performed by [kraken](http://kraken.re/) OCR solution).

| #   | name          | nb of images | GT for segmenter? | GT for recognizer? |                                                link(s) to source images |
|-----|:--------------|:------------:|:-----------------:|:------------------:|------------------------------------------------------------------------:|
| 1   | sermaises     |     (69)     |         y         |         y          |             [Archives départementales du Loiret (Sermaises)][sermaises] |
| 2   | rom-1883-1892 |     (41)     |         y         |         y          | [Archives départementales de l'Aube (Romilly-sur-Seine)][rom-1883-1892] |
| 3   | rom-1893-1902 |     (40)     |         y         |         y          | [Archives départementales de l'Aube (Romilly-sur-Seine)][rom-1893-1902] |

## Annotation system

Portions of text that are superscripted are preceded with `^` such as "1<sup>er</sup>" will be transcribed as "1^er".
If several words are superscripted, each word starts with a "^".

## How to cite

This dataset was built by Jean-François Boutet and [Jean-Pierre Merx](https://github.com/jpmjpmjpm).

The original works and their digitization are all copyright-free, but properly annotating a corpus takes time and is a
task that should be recognized. If you use any item from this corpus of ground truth, cite the dataset using the
following information:

```
title : 'GenAuto TD Corpus'
url: 'https://github.com/jpmjpmjpm/genauto-td-htr.git'
project-name: 'GenAuto'
project-website: ''
authors:
    - name: 'Boutet'
      surname: 'Jean-François'
      roles:
      - 'transcriber'
      - 'aligner'
    - name: 'Merx'
      surname: 'Jean-Pierre'
      roles:
      - 'transcriber'
      - 'aligner'
      - 'project-manager'
description: '150 transcribed images from "Tables Décennales" French Civil Registry.
Those come from Sermaises and Romilly-sur-Seine municipalities. '
language: 'French'
#other-languages:
#    - "Optional"
script: 'Latin'
script-type: 'only-manuscript'
time: 1792--1902
hands: 
    - count: 'less-than-11'
      precision: 'estimated'
license:
    - {name: 'CC-BY 4.0', url: 'https://creativecommons.org/licenses/by/4.0/'}
format: 'Alto-XML'
volume:
    - {count: "300", metric: "pages"}
    - {count: "150, metric: "images"}
```

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
[sermaises]: https://consultation.archives-loiret.fr/e/EtatCivil?from=0&f_11%5B0%5D=Tables+d%E9cennales&f_10%5B0%5D=Sermaises
[rom-1883-1892]: https://www.archives-aube.fr/ark:42751/s0057769c92e9dea/57769c92ea3cc
[rom-1893-1902]: http://www.archives-aube.fr/ark:/42751/s0057769d248ccfa/57769d248d20b
