---
layout: single
author_profile: true
permalink: /
title: "About"
---

The **"FLexible EPIdemic MOdeling Pipeline"** (*flepiMoP*; formerly known as the *COVID Scenario Modeling Pipeline* or *CSP*) is an open-source software suite designed by researchers in the [Johns Hopkins Infectious Disease Dynamics Group](http://www.iddynamics.jhsph.edu/) and at [UNC Chapel Hill](https://sph.unc.edu/epid/epidemiology-landing/) to simulate a wide range of compartmental models of infectious disease transmission. The disease transmission and observation models are defined by a no-code configuration file, which allows models of varying complexity to be specified quickly and consistently, from simple problems described by SIR-style models in a single population to more complicated models of multiple pathogen strains transmitting between thousands of connected spatial divisions and age groups.

In the context of the [COVID-19 Scenario Modeling Hub](https://covid19scenariomodelinghub.org/) and the [COVID-19 Forecast Hub](https://covid19forecasthub.org/), *flepiMoP* is used to model transmission of SARS-CoV-2 in the US at the state level using a compartmental metapopulation structure, where the fifty US states are connected through human mobility and most epidemiological processes (e.g., vaccinations, the emergence of variants, waning immunity) are simulated mechanistically. *flepiMoP* has also been modified to model influenza transmission in the US as part of the [Flu Scenario Modeling Hub](https://fluscenariomodelinghub.org/) and [FluSight](https://www.cdc.gov/flu/weekly/flusight/index.html).

However, the pipeline is much more general and can be used to simulate the dynamics of any infection that can be expressed as a [compartmental epidemic model](https://en.wikipedia.org/wiki/Compartmental_models_in_epidemiology). These include applications in chemical reaction kinetics, pharmacokinetics, within-host disease dynamics, or applications in the social sciences.

In addition to producing forward simulations given a specified model and parameter values, the pipeline can also attempt to optimize unknown parameters (e.g., transmission rate, case detection rate, intervention efficacy) to fit the model to datasets the user provides (e.g., hospitalizations due to severe disease) using a Bayesian inference framework. This feature allows the pipeline to be utilized for short-term forecasting or longer-term scenario projections for ongoing epidemics, since it can simultaneously be fit to data for dates in the past and then use best-fit parameters to make projections into the future.

*flepiMoP* source code is available on [GitHub](https://github.com/HopkinsIDD/flepiMoP). Instructions for installation, specifying models, and running simulations are available on [Gitbook](https://iddynamics.gitbook.io/flepimop/). If you have questions or concerns regarding *flepiMoP*, please contact Shaun Truelove (shauntruelove AT jhu DOT edu).
