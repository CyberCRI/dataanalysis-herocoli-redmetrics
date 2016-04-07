# data analysis for hero.coli

This repository contains a set of notebooks used to produce analysis to help optimize [hero.coli](http://herocoli.com/) and get new data about learning through science games. We are using row logs of activity coming from the [red metrics](https://redmetrics.io/) platform.

The main purpose is to provide a primer to perform data science with open software tools commonly used in the scientific field:

- [ipyton notebooks/jupyter](http://jupyter.org/): a important piece of open science allowing to combine literate programming with computing science data.
  - [pandas](http://pandas.pydata.org/): data manipulation and selection
  - [matplotlib](http://matplotlib.org/): 2D plotting library
  - [scikit-learn](http://scikit-learn.org/): machine learning implementation of common algorithms

## hero.coli

[Hero.coli](http://herocoli.com/) is an exploration game about synthetic biology. It uses the main concept of this scientific science and incentive players to craft/assemble biobricks to reach new steps in the main level.

![hero.coli alpha version screenshot](http://herocoli.com/img/erocoli-screen01.jpg)

The current lead contributor of this project is the Raphael Goujet ([CRI](http://cri-paris.org)).

## datasets

- [players statistics (csv)](https://github.com/CyberCRI/dataanalysis-herocoli-redmetrics/blob/master/data/players_stats.csv): 156 games ([notebook](data/0.1. compile basic data about players~games.ipynb))
- [coordinates of events (csv)](https://github.com/CyberCRI/dataanalysis-herocoli-redmetrics/blob/master/data/players_coordinates.csv): 2010 events ([notebook](data/0.2. compile paths.ipynb))

## analysis

### hot spots of the main level

![hotspot map](https://github.com/CyberCRI/dataanalysis-herocoli-redmetrics/raw/master/images/map.hotspots.png)

If you are curious about it, you can check the notebook where we [are generating the maps](2. paths.ipynb).

### player profiling

We also perform a series of regressions to get an idea about player profiles but there is not enough data yet to reach conclusive statements.

We could for example [try to predict if a player is going to complete the game or not](1.1.%20predicting%20if%20a%20player%20is%20going%20to%20complete%20the%20game%20or%20not.ipynb).

You can check [the notebook](1. basic player statistics.ipynb) if you are looking for examples about how to use pandas to manipulate data in coordination with machine learning implentation (via scikit-learn)

## fun facts

- no player than played with the sandbox have completed the game.

## diagnostics

- attention span: players who are completing the game tend to play around ~800 seconds. There is a drop after 15 minutes of play.
- need more data to get significant results.
