---
layout: page
title: Projects
---

## Project 1:

Due *30 Jan, 13:00*

   - *Reading* Chapter 1 Baines
   - *Technical*:  
      - Setup computer to run MITgcm in parallel [See here](./install/)
      - Download [MITgcm](http://mitgcm.org) and install
      - Setup and run a simple test case: mean stratified flow over a Gaussian bump (See Klymak et al 2010, *JFM*, but w/ less resolution).  Use [This repository](https://github.com/jklymak/MITgcmExampleSteadyGauss) as your starting point and see the instructions in the `README.md`
      - Plot the result of the model showing snapshots as the model spins up.
      - Do two more runs with `Fr =  0.13, 0.39` and do a qualitative (plot) comparison with the base case.  
   - *Hand in*:
      - A github repository link to your *modified* code.  For an mitgcm run this usually means the `code`, and `input` directories.  No need to 
      - A [jupyter](http://jupyter.org) notebook with your plots in it.  Preferably served from github.
