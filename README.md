# README.md Teaching-Strathclyde-BM405

## Overview

This repository contains materials for a guest lecture on microbial
comparative genomics, first delivered 21st November 2014, at the University
of Strathclyde.

* 2014-11-21: First delivery
* 2015-11-13: Second delivery

## Building slides/handouts

Production of slides/handouts is automated in a `Makefile` that has options to build all sections individually with, e.g.

```    
make part1_slides.pdf
make part1_handouts.pdf
make part1
```
 
These commands build the slides, the handouts, and both slides *and* handouts for part1.
    
Slides and handouts concatenating all the sections with a unified table of contents can be built with:
    
```
make BM405_slides.pdf
make BM405_handouts.pdf
``` 
    
All of the slides/handouts can be built in one go with
    
```
make slides
make presentation
make handouts
make all
```

Intermediate/auxiliary file cleanup is handled automatically in the makefile, but can be forced with:
    
```
make clean_intermediates
```

All output files can be removed with
    
```
make clean
```