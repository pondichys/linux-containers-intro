# Linux Container - Introduction

This repository contains slides of a presentation given at the DevOps guild of STIB-MIVB.

This is an introduction to Linux containers for non-technical people that aims at explaining what problems do containers solve.

Many slides come from Jerôme Petazzoni's self-paced [Introduction to Docker and Containers](https://container.training/intro-selfpaced.yml.html) training.

## Technical stuff

The slides are written in Markdown and they are available as HTML pages using [Reveal.js](https://revealjs.com/). The branch `gh-pages` of this repository contains all static files needed to publish these slides automatically as Github pages.

The slides are publicly available at https://pondichys.github.io/linux-containers-intro/

Use the instructions below if you want to present these slides without internet connectivity and have python installed on your machine:

1. Go to the root of the local copy of this repository

1. Checkout the `gh-pages` branch

1. Run `python -m http.server 8080` or `python3 -m http.server 8080` depending on how python is available on your computer.

1. Open your web browser to http://localhost:8080 to navigate in the presentation.