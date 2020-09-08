---
layout: post
title:  "Seismic harmonic response of inhomogeneous soil: scaling analysis"
date:   2020-09-04 17:18:56 -0700
categories: jekyll update
--- 

The article titled ["Seismic harmonic response of inhomogeneous soil: scaling analysis"](https://www.icevirtuallibrary.com/doi/abs/10.1680/jgeot.19.P.042) was my very first paper and my first contribution to One-dimensional Site Response Analysis (1DSRA). I should add Linear-Elastic to that, so LE-1DSRA.

This work provided me a chance to revisit previous results by [Rovithis et al.](https://www.sciencedirect.com/science/article/pii/S026772611100008X?casa_token=p3zYnb0UG7IAAAAA:FjrRbpk1s11X9j09kUd-6rSJbZA0sYjg-8D7ipZlwtoMMXTzV4CMsJLdHMoRnK1H5zkjNVMxFiA). 
There was a number aspects of their contribution that got my attention, in particular, everything concerning the deinition of the equivalent-homogeneous properties (the other feature reported in the paper that I have explored is the "surface energy concentration phenomenon").

# The gist

Allow me to give my definition of "equivalent homogeneous properties": those that render of a homogeneous soil layer the response alike the one of the inhomogeneous deposit. When it comes to define "the response", I refer to either natural frequencies or amplitudes.  In practice, the shear-vave velocity, Vs, is the heterogeneous mechanical property we focus on, although it can be splitted into shear modulus and density, and depth-evolving material damping can be considered as well.

This work, which is centered around the so-called "generalized parabola distribution of shear wave velocity" gave me a chance to bring considerations of Asymptotic Analysis and Perturbation Theory to the study of the problem. Namely, in first place, the influence of the two dimensionless parameters that define the "generalized parabola" was explored, and secondly (and more interestingly) the short-wavelength/high-frequency limit was studied by taking the ratio between characteristic magnitudes of inertial and elastic forces to infinity.

Concerning the aforementioned two parameters, it was found that, for some cases, the contrast between rock bottom and free-surface stiffnesses controls the shape of the base-to-top displacement transfer function.

The dimensionless parameter r can be interpreted in different ways: 
* The most obvious one is as the ration between the externally-imposed excitation frequency and a characteristic frequency of the system (Vref/4H, to be precise). Hence when r is much smaller than 1, we are in a quasi-static regime, where elastic forces are in charge of balancing the shaking; when r is order 1, the elastic forces and the inertial forces are of the same order (fundamental resonance); finally, when r much greater than 1, the inertial forces are in charge balancing the external load, we are therefore in the domain of the higher modes, so to speak. 
* Likewise, a geometrical interpretation is also feasible: r furnishes the ratio between the height of the layer and the wavelength of the standing wave. If r is small in comparison to 1, we are in the long-wavlength regime (the excitation varies slowly within the layer, thus it resembles a rigid body motion in first approximation)
* Simply acknowledging how r appears in the equation of motion, one recognizes r (squared) as the ratio between inertial and elastic forces.

The prior presentation of r is motivated on the basis of this parameter being the one we focus on in the second part of the paper. It was shown that, by taking the limit as it tends to infinity, the analytical solutions simplify greatly. For once, all the Bessel functions collapse into secant function times a constant plus extra terms order 1 over r (thus, these terms vanish in the limit). The function of the inhomogeneoty distribition that appears in the argument of the secant is precisely equivalent to the harmonic mean of the distribution, what renders what is also called "averaged-time equivalent shear wave velocity". The 
This proved unequivocally that:
* Sites whose shear-wave velocity distribution can be described by means of the generalized parabola behave alike a homogeneous one, whose shear-wave velocity corresponds to the harmonic mean and whose amplitude is scaled by the square root of the ratio velocity of soil at the bottom over velocity of soil at the free surface.
* The approximation works better the higher the mode, but it is unable to capture the fundamental mode (except in sites with very mild heterogeneity, i.e., almost homogeneous), since in that case r is order 1 (it does not tend to infinite by any means!).  

# Follow-up work

This contribution open two research paths that I have been exploring since:
1. Generalization of the short-wavelength result: we can prove that the harmonic mean appears naturally in the case of generalized-parabola distribution, but what conditions are truly necessary for this limit behavior to occur. Spoiler: as long as the evolution is described by a C1-function (i.e. continuous function with continuoous first derivatives), this [will always be the case](https://engrxiv.org/db7jv/). This will be the subject of a future post. 
2. A different definition of equivalent-homogeneous site is necessary for lower frequency ([fundamental mode](https://www.sciencedirect.com/science/article/abs/pii/S0267726119314599)).  