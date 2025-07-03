# Lyman-Break Galaxy Clustering Investigation  <br />
Human-AI Collaboration Project  <br />
Center for Data-Driven Discovery <br />
Kavli IPMU


![alt text](wpxi_UM_sSFR_Bielby_plot.png)


<h1><b> Relevant Links: </b></h1>  <br />
<ul>
<li><a href="https://skun.iaa.csic.es/SUsimulations/UchuuDR2/Uchuu_UM/">Uchuu UM snapshot data and Readmes.</a></li> <br />
<li><a href="https://corrfunc.readthedocs.io/en/master/index.html">Corrfunc, python package used to measure 2PCFs.</a></li> <br />
  
</ul>

<h1><b> Relevant Papers: </b></h1>  <br />

-- In line with our investigation: They created simulated LAE/LBG mocks and used field-level EFT to model the simulated observations.<br />
<b>High-redshift Millennium and Astrid galaxies in effective field theory at the field level</b></br>
<i> Sullivan+ 2025 </i> <br />
<a href="https://arxiv.org/abs/2505.03626">https://arxiv.org/abs/2505.03626</a> <br />
In this paper we measure the bias parameters and other EFT coefficients from samples of two types of star-forming galaxies in the state-of-the-art MilleniumTNG and Astrid hydrodynamical simulations. Our measurements are based on the field-level EFT forward model that allows for precision EFT parameter measurements by virtue of cosmic variance cancellation. Specifically, we consider approximately representative samples of Lyman-break galaxies (LBGs) and Lyman-alpha emitters (LAEs) that are consistent with the observed (angular) clustering and number density of these galaxies at z=3. Reproducing the linear biases and number densities observed from existing LAE and LBG data, we find quadratic bias parameters that are roughly consistent with those predicted from the halo model coupled with a simple halo occupation distribution model.<br />

-- Similar to what our observation will be like of the LBGs in the PFS:GE. Details the selection function of LBGs, their redshift distributions, and measures the clustering signal (projected and 3D 2PCF). Models the clustering signal to constrain growth-rate of large-scale structure. <br />
<b>The VLT LBG Redshift Survey - III. The clustering and dynamics of Lyman-break galaxies at z ~ 3</b></br>
<i> Bielby+ 2013 </i> <br />
<a href="https://arxiv.org/abs/1204.3635">https://arxiv.org/abs/1204.3635</a> <br />
We present a catalogue of 2135 galaxy redshifts from the VLT LBG Redshift Survey (VLRS), a spectroscopic survey of z ~ 3 galaxies in wide fields centred on background quasi-stellar objects. We have used deep optical imaging to select galaxies via the Lyman-break technique. Spectroscopy of the Lyman-break galaxies (LBGs) was then made using the Visible Multi-Object Spectrograph (VIMOS), giving a mean redshift of z=2.79. We analyse the clustering properties of the VLRS sample and also of the VLRS sample combined with the smaller area Keck-based survey of Steidel et al.<br />

-- Ben's diffHOD technique that we would like to employ when modelling the observations with the HOD. <br />
<b>Differentiable Stochastic Halo Occupation Distribution</b><br />
<i> Horowitz+ 2022 </i> <br />
<a href="https://arxiv.org/abs/2211.03852">https://arxiv.org/abs/2211.03852</a> </br>
In this work, we demonstrate how differentiable stochastic sampling techniques developed in the context of deep Reinforcement Learning can be used to perform efficient parameter inference over stochastic, simulation-based, forward models. As a particular example, we focus on the problem of estimating parameters of Halo Occupancy Distribution (HOD) models which are used to connect galaxies with their dark matter halos. We demonstrate our technique on a mock galaxy catalog generated from the Bolshoi simulation using the Zheng et al. 2007 HOD model and find near identical posteriors as standard Markov Chain Monte Carlo techniques with an increase of ~8x in convergence efficiency.  </br>

-- Our investigation will employ tactics similar to this paper, where we shuffle galaxies between halos with the same host mass to remove the assembly bias signal and determine our ability to model the clustering signal when an assembly bias is present and when it has been removed. <br />
<b>The Effects of Galaxy Assembly Bias on the Inference of Growth Rate from Redshift-Space Distortions</b>  <br />
<i> McCarthy+ 2019 </i> <br />
<a href="(https://arxiv.org/abs/1810.05183)">https://arxiv.org/abs/1810.05183</a> <br />
The large-scale redshift-space distortion (RSD) in galaxy clustering can probe fσ8, a combination of the cosmic structure growth rate and the matter fluctuation amplitude, which can constrain dark energy models and test theories of gravity. While the RSD on small scales (e.g. a few to tens of h−1Mpc) can further tighten the fσ8 constraints, galaxy assembly bias, if not correctly modelled, may introduce systematic uncertainties. Using a mock galaxy catalogue with built-in assembly bias, we perform a preliminary study on how assembly bias may affect the fσ8 inference.

-- An example of measuring the projected 2PCF of LBGs from photometric observations. Shows what the HOD model will allow us to learn from such an observation. <br />
<b> The Galaxy--Halo Connection in High-Redshift Universe: Details and Evolution of Stellar-to-Halo Mass Ratios of Lyman Break Galaxies on CFHTLS Deep Fields </b><br />
<i> Ishikawa+ 2017 </i> <br />
<a href="https://arxiv.org/abs/1612.06869">https://arxiv.org/abs/1612.06869</a> </br>
We present the results of clustering analyses of Lyman break galaxies (LBGs) at z∼3, 4, and 5 using the final data release of the Canada--France--Hawaii Telescope Legacy Survey (CFHTLS). Deep- and wide-field images of the CFHTLS Deep Survey enable us to obtain sufficiently accurate two-point angular correlation functions to apply a halo occupation distribution analysis. <br />

-- A detailed description of the properties of LBGs and what a potential future spectroscopic survey might look like. Good for a background about LBGs. <br />
<b> Cosmology with dropout selection: Straw-man surveys & CMB lensing </b> <br />
<i> Wilson and White 2019 </i> <br />
<a href="(https://arxiv.org/abs/1904.13378)">https://arxiv.org/abs/1904.13378</a> <br />
Focusing on color-color selection, we estimate the completeness, contamination, and spectroscopic survey speed of tailored Lyman-break galaxy (LBG) samples. We forecast the potential of CMB lensing cross-correlation, clustering redshifts and Redshift-Space Distortions (RSD) analyses. In particular, we estimate: the depth dependence of interlopers based on CFHTLS data and propagate this to biases in cosmology; new inferences of (non-linear) halo bias at these redshifts and depths using legacy data; detailed forecasts of LBG spectra as would be observed by DESI, PFS, and their successors.<br />

-- Do mergers have a significant impact on SFR in observations? How important will knowing the merger histories of the LBG systems be when modeling the target selection?  <br />
<b>Effect of galaxy mergers on star formation rates</b>  <br />
<i> Pearson+ 2019 </i> <br />
<a href="(https://arxiv.org/abs/1908.10115)">https://arxiv.org/abs/1908.10115</a> <br />
We aim to determine the effect of galaxy mergers on the SFR of galaxies using statistically large samples of galaxies, totalling over 200,000, over a large redshift range, 0.0 to 4.0. We train and use convolutional neural networks to create binary merger identifications (merger or non-merger) in the SDSS, KiDS and CANDELS imaging surveys. We then compare the galaxy main sequence subtracted SFR of the merging and non-merging galaxies to determine what effect, if any, a galaxy merger has on SFR. We find that the SFR of merging galaxies are not significantly different from the SFR of non-merging systems. The changes in the average SFR seen in the star forming population when a galaxy is merging are small, of the order of a factor of 1.2. <br />

-- An investigation into how the merger histories of LBG systems can impact the UV luminosity function and the SFR density. Gives us a physical understanding of how SFR can impact LBG selection, since it is the bright UV continuum that is detected and which galaxies have bright UV continuum will be informed by the specifics of galaxy formation. <br />
<b>The evolution of Lyman-break galaxies in CDM </b><br />
<i> Lacey+ 2010 </i> <br />
<a href="(https://arxiv.org/abs/1004.3545)">https://arxiv.org/abs/1004.3545</a> <br />
We make a detailed investigation of the properties of Lyman-break galaxies (LBGs) in the LambdaCDM model. We present predictions for two published variants of the GALFORM semi-analytical model: the Baugh et al. (2005) model, which has star formation at high redshifts dominated by merger-driven starbursts with a top-heavy IMF, and the Bower et al. (2006) model, which has AGN feedback and a standard Solar neighbourhood IMF throughout. We show predictions for the evolution of the rest-frame far-UV luminosity function in the redshift range z=3-20, and compare with the observed luminosity functions of LBGs at z=3-10.

-- The galaxy mock catalog that we will start our investigation with. I will also include details about this mock in the relevant notebook (TBD). <br />
<b>The Uchuu-UniverseMachine dataset: Galaxies in and around Clusters</b> <br />
<i> Aung+ 2022 </i> <br />
<a href="(https://arxiv.org/abs/2209.12918)">https://arxiv.org/abs/2209.12918</a> <br />
We present the public data release of the Uchuu-UM galaxy catalogues by applying the UniverseMachine algorithm to assign galaxies to the dark matter halos in the Uchuu N-body cosmological simulation. It includes a variety of baryonic properties for all galaxies down to ∼5×108M⊙ with halos in a mass range of 1010<Mhalo/M⊙<5×1015 up to redshift z=10.

-- Some specifics of the observed properties of LBGs from HSC observations and a measurement of the projected 2PCF, modelled with the HOD and a non-linear HOD. <br />
<b>GOLDRUSH. II. Clustering of galaxies at z = 4–6 revealed with the half-million dropouts over the 100 deg^2 area corresponding to 1 Gpc^3</b> <br />
<i> Harikane+ 2018 </i> <br />
<a href="(https://academic.oup.com/pasj/article/70/SP1/S11/4662843)">https://academic.oup.com/pasj/article/70/SP1/S11/4662843</a> <br />
We present clustering properties from 579492 Lyman-break galaxies (LBGs) at z = 4–6 over the 100 deg2 sky (corresponding to a 1.4 Gpc3 volume) identified in early data of the Hyper Suprime-Cam (HSC) Subaru Strategic Program survey. We derive angular correlation functions (ACFs) for the HSC LBGs with unprecedentedly high statistical accuracies at z ∼ 4–6, and compare them with the halo occupation distribution (HOD) models. We clearly identify significant ACF excesses in 10″ < θ < 90″, the transition scale between one- and two-halo terms, suggestive of the existence of the non-linear halo bias effect. Combining the HOD models and previous clustering measurements of faint LBGs at z ∼ 4–7, we investigate the dark matter halo mass (Mh) of the z = 4–7 LBGs and its correlation with various physical properties including the star formation rate (SFR), the stellar-to-halo mass ratio (SHMR), and the dark matter accretion rate (⁠dMh/dt) over a wide mass range of Mh/M⊙  = 4 × 1010–4 × 1012. 

-- Compares the 'observed' star-formation history (SFH) of Lyman-alpha emitters to LBGs. Some details about the SFH of LBGs from observations.<br />
<b>ODIN: Star Formation Histories Reveal Formative Starbursts Experienced by Lyman Alpha Emitting Galaxies at Cosmic Noon</b><br />
<i> Firestone+ 2025 </i> <br />
<a href="(https://arxiv.org/abs/2501.08568)">https://arxiv.org/abs/2501.08568</a> <br />
In this work, we test the conventional assumption that Lyman Alpha Emitting galaxies (LAEs) are experiencing their first major burst of star formation at the time of observation. ...suggests that LAEs have more complicated stellar mass assembly than expected. We also find that the fraction of total stellar mass created in the last 200 Myr is ~1.33 times higher in LAEs than in control Lyman Break Galaxy (LBG) samples, and that a majority of LBGs are experiencing dominant bursts, reaffirming that LAEs differ from other star forming galaxies. Overall, our results suggest that multiple evolutionary paths can produce galaxies with strong observed Lyα emission.

-- Use semi-analytic models to predict the angular correlation function and compare to HOD. Gives some possible forms of the HOD for LBGs.<br />
<b>The clustering and halo occupation distribution of Lyman-break galaxies at z∼4</b><br />
<i> Park+ 2015 </i> <br />
<a href="https://arxiv.org/abs/1511.01983">https://arxiv.org/abs/1511.01983</a> <br />
We investigate the clustering of Lyman-break galaxies (LBGs) at z∼4. Using the hierarchical galaxy formation model GALFORM, we predict, for the first time using a semi-analytical model with feedback from active galactic nuclei (AGN), the angular correlation function (ACF) of LBGs and find agreement within 3σ with new measurements of the ACF from surveys including the Hubble eXtreme Deep Field (XDF) and CANDELS field. By analysing the halo occupation distribution (HOD) predicted by the model, we find evidence that AGN feedback affects the HOD of central LBGs in massive haloes. We investigate the effect of photometric errors in the observations on the ACF predictions. We find that the observational uncertainty in the galaxy luminosity reduces the clustering amplitude and that this effect increases towards faint galaxies, particularly on small scales. To compare properties of model with observed LBGs this uncertainty must be considered.

