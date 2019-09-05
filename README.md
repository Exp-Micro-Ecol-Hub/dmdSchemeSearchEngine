Search Engine for `dmdScheme` MetaData
================

# Summary

This document outlines the requirements for a search engine which should
search the metadata to identify and return the data or a reference to
the data based on the search term.

Initially, it will only be a basic mockup search engine, but can, at a
later stage, lead to a fully fledged shiny app which can be a first stop
for the search in dmdSchemes.

# Requirements

## How to submit new MetaData and data files

A button

## What to search for

Based on the metadata in **`dileptus_expt_emeScheme_095.xlsx`**

  - [ ] a) individual properties (i.e. values in cells of the
    spreadsheet)?
      - `Species$name = "Colpidium striatum"`  
      - `Species$source = "Carolina Biological Supply, Burlington, USA"`
      - `Experiment$temperature = 22`
  - [ ] b) combinations of cells in a column?
      - `Species$name = "Dileptus anser" && Species$functionalGroup =
        bacterivore`
      - `Species$name = "Dileptus anser" || Species$functionalGroup =
        bacterivore`
  - [ ] combination of a) and b) combined by `AND` (`&`) and `OR` (`|`)
    and `()`

## What to return

  - show file name
  - button to download data file(s)
  - DOIs of data files so that they can be downloaded from external
    repository (e.g. Zenodo)

# Tool to use

The initial implementation will be done in R as a shiny app.
