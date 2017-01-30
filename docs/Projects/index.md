---
layout: page
title: Projects
---

## Project 2:

Due *14 Feb, 13:00*

   - *Reading* Chapter 2, Baines.
   - *Section 2.3*:
   - *numerically* reproduce Figure 2.6 for $F_0 = 0.8$ and $F_0 = 1.2$.  Note, do this by solving the characteristic equations (not a fully non-linear MITgcm run).  Plot the interface height at a few times in the flow, and discuss the shock formation.
   - In MITgcm, run the same two simulations and see if they agree.  For these runs, the best idea is to use a "reduced gravity" simulation with two layers of slightly different densities, and with a very thick upper layer. This will approxiate a surface wave flow.
   - Examine how well the jump condition (pg 37) is approximated in    this flow (i.e. $c_J$ and the energy lost).
   - *Simulate* a flow from each of the regions in the flow diagram    Fig 2.11 and veritfy that you get the expected behaviour.

*NOTE* You may need to use more resolution.  For z, suggest stretching your grid in the vertical away from the region of interest near the bottom so you have lots of mass up there, but not much computation.

*NOTE* Make sure your results have some commentary. Practice describing what you are seeing and making preliminary conclusions.


   




## Project 1:

Due *30 Jan, 13:00*

   - *Reading* Chapter 1 Baines
   - *Technical*:  
      - Setup computer to run MITgcm in parallel [See here](https://jklymak.github.io/MITgcmExampleSteadyGauss/install.html)
      - Download [MITgcm](http://mitgcm.org) and install
      - Setup and run a simple test case: mean stratified flow over a Gaussian bump (See Klymak et al 2010, *JFM*, but w/ less resolution).  Use [This repository](https://github.com/jklymak/MITgcmExampleSteadyGauss) as your starting point and see the instructions in the `README.md`
      - Plot the result of the model showing snapshots as the model spins up.
      - Do two more runs with `Fr =  0.13, 0.39` and do a qualitative (plot) comparison with the base case.  
   - *Hand in*:
      - A github repository link to your *modified* code.  For an mitgcm run this usually means the `code`, and `input` directories.  No need to
      - A [jupyter](http://jupyter.org) notebook with your plots in it.  Preferably served from github.

