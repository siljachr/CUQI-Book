# Cochlear aqueduct advection and diffusion inferred from computed tomography imaging with a Bayesian approach

## Summary

Fluid flow and transport of therapeutic agents and pathogenic bacteria into the cochlea has been challenging to study due to its small size and location within bone. We here take advantage of recent non-invasive Computed Tomography (CT) imaging of tracer transport to infer transport parameters in a 1-dimensional advection-diffusion model of the cochlear aqueduct using a Bayesian approach.

We develop a hierarchical Bayesian inversion framework in which we combine the CT tracer data and the 1-dimensional model to infer the model advection and spatially-varying diffusion parameters. The noise level of the CT data is inferred as part of the inversion using a hyperparameter. We characterize the posterior distribution of these parameters using NUTS within Gibbs sampling. We verify our inference by comparing the model-predicted tracer concentration to the CT data and by comparing the inferred parameters to literature values. We validate our framework using synthetic data generated from the advection-diffusion model with known parameters. We use CUQIpy to implement the Bayesian inversion framework.

The evolution of the concentration of tracer in the cochlear aqueduct is well predicted by the advection-diffusion model using inferred parameters. Though diffusion of the small CT tracer varies along the aqueduct, it is usually near the free diffusion and therefore not likely to be influenced much by membranes or flow. Advection is inferred near zero in most cases. We show how to use these results to calculate transport through cochlear aqueduct for other animals and molecules.

Free diffusion dominates transport of small molecules in the cochlear aqueduct, which can therefore be effectively approximated using simple 1-dimensional (advection-)diffusion formulas.

<figure>
<img src="figures/fig_inference.png" alt="Parameter inference" width="600"/>
<figcaption>Inferred spatially-varying diffusion, noise level and advection speed in two animals, mouse 3 left ear and mouse 4 right ear.</figcaption>
</figure>

## Resources
- Paper: {cite}`Alghamdi2025CochlearAqueduct`
- Paper code GitHub repository: https://github.com/CUQI-DTU/Paper-Cochlear


