---
layout: page
title: Projects
mathjax: true
---

## Project 4:  

Due *1 May, 09:00*

  - *Reading& Chapter 3.6, 3.11
### Unidirectional flow:
  - In the MITgcm, simulate three different values of $r_1$, with three different $F_0$ and $h_m$.  When you choose what parameters to use for your simulations, try to choose partially blocked situations where the flow goes transcritical over the sill crest.  Describe the response in terms of the composite Froude number, and try to make sure you have an example of "approach control" (i.e. as in Fig 3.11).  Be sure to describe the transiet response and how the critical conditions set up.
### Exchange Flow:
  - Do three runs of an exchange flow over an obstacle.  Have a large reservoir on both sides with a dense and ligh reservoir.  For the three runs make the upper layer of light water get thicker in the dense basin and show the transition from maximal exchange to sub maximal exchange as the upper layer gets thicker. 

## Project 3:

Due *6 Mar, 13:00*

   - *Reading* Chapter 3, Baines.
   - *Section 3.3 & 3.5*:
   - *numerically* use the Rieman invariants (Eq 3.3.13) to get solutions for an initial smoothed tophat interface displacement, with zero velocity anomaly from the background shear flow (By a smoothed step, I mean let the edges of the tophat  be initially smoothed so that if any shocks develop they develop as the flow evolves, not right away). Explore at least 4 locations in the parameter space shown in Fig 3.2.  For each location in parameter space explore what happens as your initial $\eta$ is positive or negative.  (I'll admit I have not carried out this exercise, but I *think* that for some interface displacements you will get the interface displacement changing sign within a few wavelengths).  Also make sure you find a couple of examples where shocks form.  
   - In MITgcm, run the same simulations and see if they agree.
   - In the MITgcm set up some hydraulic jumps and trace out one of the curves in Fig 3.7 for *two* values of $r_u$.  
     - Note the upstream changes (so you can't really specify $r_d$ very easily)
     - Document the jump speed, and compare to the curves in 3.7 (which you should be able to draw on analytically)
     - Make sure you run the model past the maximum value of $r_d$.  

*NOTE* You will probably need to run quite a few model runs to get the above to work.  Start to develop skills in running and analyzing these automatically.  Also, in your writeup, show *example* runs, but then summarize all the runs in one or two plots.

*NOTE* Make sure your results have some commentary. Practice describing what you are seeing and making preliminary conclusions.


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
