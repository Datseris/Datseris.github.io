---
layout: single
title: "Research"
permalink: /research/
author_profile: true
redirect_from:
  - /research
---

My research interests can be summarized as follows:

* Low dimensional chaos and Hamiltonian chaos
* Dynamical billiards and their role in electron transport
* Nonlinear timeseries analysis of climate-related observations
* Conceptual climate models
* Music timeseries analysis and the dynamics of music
* Education of nonlinear dynamics

The physics I was studying in my PhD was electron transport in nanodevices, both quantum and classical. For my postdoc I am turning the scales up a notch and look at planetary albedo. Throughout my career in parallel to the core physics research, I perform
Most of my research is on physics: electron transport, nonlinear dynamics and chaos, climate physics. I also work on music timeseries analysis.

*this page only lists currently active research projects, finished projects are published (see "Publications")*

Active projects:

* [Albedo symmetry](#albedo-hemispheric-symmetry)
* [Synchronization between musicians](#synchronization-between-musicians)
* [Nonlinear dynamics education](#nonlinear-dynamics-education)

## Albedo hemispheric symmetry

The albedo of the Earth is the ratio of the outgoing to incoming shortwave radiation, i.e. the percentage of the Sun's radiation that is reflected by the Earth. Recent satellite observations provided by [CERES](https://ceres.larc.nasa.gov/) made it possible to accurately describe this quantity on a planetary scale. Surprisingly, it turns out that once averaged across the north and south hemisphere, the Earth's albedo only differs by 0.08%, which given the error margins, means that there is a hemispheric symmetry. To see this, one can compute the hemispheric difference of the zonally and yearly averaged outgoing solar radiation (which is directly proportional to the albedo), which is shown in the following figure:

![](../files/plots/hemispheric_symmetry.png)

While different latitudes are clearly non-symmetric, integrating over latitude gives a total difference of ≈0.08%, meaning that there is a **hemispheric symmetry**. This is extremely surprising, because the hemispheric land and sea contents differ dramatically. We know that the symmetry exists because clouds exists, because without clouds the aforementioned difference is in fact not ≈0.08% but ≈11%. However, we don't know how or why it happens, or even whether it exists by pure chance.

In this project I am trying to quantify this symmetry and clarify if it is a result of chance. I want to find out not only why it exists (assuming the most likely scenario that it is *not* by chance), but also how. My end-goal with this project is a conceptual climate model, based on basic energy balance considerations and the (stable) surface albedo, that can reproduce the hemispheric symmetry.

## Synchronization between musicians
Music is perhaps the biggest cultural achievement of humanity. But music is also a very complex, and complicated process. This is because of the huge number of factors involved. Besides the actual music notes themselves, a process at least three dimensional (time, intensity, pitch), there is also human interaction, expression, and improvisation. Yet, what has become clear in recent years, is that the timeseries of human music performances are underlined by seemingly universal mathematical patterns. For example, the timeseries of timing, intensity, and even pitch fluctuations seem to be accurately represented by pink noise processes: they are random, but also with power-law-like temporal correlations. I describe all of these findings in an invited talk I gave at the University of Nottingham, which is [available on YouTube](https://www.youtube.com/watch?v=9wzr5DFHJ48).

What I am currently interested in is how musicians synchronize. For example, the following plot comes from a recording of "Heard it through the grapevine" that I have played with the keyboard player of my band (see the "Music" page if you are interested). The x-axis is simply time, while the y-axis shows the temporal deviations of the played notes of either drums (blue) or piano (orange).

![](../files/plots/mtds.png)

While its clear that these timeseries are "random" (this pink noise we mentioned above), it is also clearly that they are very much dependent on each other. The fluctuations go up and down together, and this happens because the two musicians are "synchronized" with each other. I am currently analyzing the nature of this synchronization, and how it can exist in such a setting, where the timing of the musicians have a stochastic nature. I am also interested in understanding how a metronome affects this synchronization. Musicians generally agree that it is easier to synchronize with each other in the *absence* of a metronome. From a scientific perspective, the opposite should be true: since the timings of humans are stochastic, having a purely deterministic perfectly periodic signal should make synchronization easier. That's not the case, but why and how? To answer these questions I perform experiments, recording musicians and then analyzing the recorded timeseries.

## Nonlinear dynamics education
Chaos theory is arguably one of the most beautiful frameworks to approach the world, at least from the mathematics perspective. However, nonlinear dynamics, the root of chaos theory, are very rarely tractable analytically. Thus, a "nonlinear dynamicist" always works hand-in-hand with a computer.

There are dozens of textbooks on nonlinear dynamics. Oddly enough, none of them takes computer code seriously. I believe this should be changed, and education of nonlinear dynamics should occur simultaneously with code. Technology has thankfully advanced enough to allow one to solve complicated problems while writing concise, expressive, high level code. I am aiming to take advantage of this progress into a new introductory textbook about nonlinear dynamics I am co-authoring with Prof. [Ulrich Parlitz](https://www.uni-goettingen.de/en/105320.html). To give you an idea, here are to excerpts. In the fist one, a real, runnable implementation of an algorithm to compute the maximum Lyapunov exponents is shown in text as a special "Code" environment, like a "Figure" or "Table" environment:

![](../files/plots/book1.PNG)

In the second excerpt we show a figure of how the entropy of a chaotic set changes with the partition size. Next to the figure is the *full code necessary to reproduce it*.

![](../files/plots/book2.PNG)

All of this is possible for two reasons: first, the code snippets use a high-level expressive new language designed for scientific computing called [Julia](https://julialang.org/). The second reason is the existence of an award-winning software library for nonlinear dynamics and chaos, called [DynamicalSystems.jl](https://juliadynamics.github.io/DynamicalSystems.jl/dev/) that I wrote while developing scientific software (see the "Software" page for more).

Having such a book comes with tremendous advantages: the students don't have to spend hours, or even days, writing a code implementation of an algorithm they read about, and they can instead experiment with it immediately. In addition this way there is education about code, which for a nonlinear dynamicist is certainly "half part of the job".
