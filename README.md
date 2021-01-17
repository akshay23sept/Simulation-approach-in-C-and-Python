# Simulation-approach-in-C
## A <code>Lattice-Boltzmann method (LBM)</code> based approach to study Eulerian-Lagrangian fluid dynamics
![alt text](https://github.com/akshay23sept/Simulation-approach-in-C-and-Python/blob/master/images/example.png)
<h2><a id="user-content-introduction" class="anchor" aria-hidden="true" href="https://github.com/akshay23sept/Simulation-approach-in-C-and-Pythonintroduction"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Introduction:</h2>
<div><pre><span>.</span>
<p>A general purpose <em>Lattice-Boltzmann</em> code for fluid-dynamics simulations. The code includes :</p>
├── <strong>fluid dynamics</strong> with several volume forcing terms for
│&nbsp;&nbsp; ├──<code>channel flow</code> 
│&nbsp;&nbsp; ├──<code>homogeneous isotropic turbulence (HIT)
│&nbsp;&nbsp; ├──<code>buoyancy)</code>
├── <strong>temperature dynamics</strong> 
│&nbsp;&nbsp; ├──<code>advection</code> 
│&nbsp;&nbsp; ├──<code>diffusion</code>
│&nbsp;&nbsp; ├──<code>sink/source or reaction terms)</code>
├── <strong>phase change</strong> 
│&nbsp;&nbsp; ├──<code>enthalpy formulation for solid/liquid systems</code> 
├── <strong>scalar transport</strong> 
│&nbsp;&nbsp; ├──<code>same functionalities as temperature</code> 
├── <strong>lagrangian dynamics</strong> 
│&nbsp;&nbsp; ├──<code>tracers</code> 
│&nbsp;&nbsp; ├──<code>non-shperical Jeffery rotation</code> 
│&nbsp;&nbsp; ├──<code>gyrotaxies</code> 
│&nbsp;&nbsp; ├──<code>heavy/light &amp; active  point-like particles</code> 
├── <strong><code>Large Eddy Simulation (LES)</code></strong> 
│&nbsp;&nbsp; ├──<code>Smagorinsky</code> 
│&nbsp;&nbsp; ├──<code>shear improved Samgorinsky with Kalman filter</code> 
<h2><a id="user-content-introduction" class="anchor" aria-hidden="true" href="https://github.com/akshay23sept/Simulation-approach-in-C-and-Python#Prerequisite:"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Prerequisite:</h2>
<ol>
<li>Python 2.7 or above</li>
<li>C++</li>
<li>HDF5</li> 
<li>MPI</li>
<li>CMake</li>
</ol>
<h2><a id="user-content-introduction" class="anchor" aria-hidden="true" href="https://github.com/akshay23sept/Simulation-approach-in-C-and-Python#Issues:"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Issues:</h2>
<ol>
Feel free to raise an issue at <a href="https://github.com/akshay23sept/Simulation-approach-in-C-and  Python">https://github.com/akshay23sept/Simulation-approach-in-C-and-Python</a>
</ol>
</h1>
<p align="center"> DNS study to analyze dynamics of diatoms in turbulent flows</p><br>
<p><a target="_blank" rel="noopener noreferrer" href="https://github.com/akshay23sept/Simulation-approach-in-C-and-Python/blob/master/images/active_particles.gif"><img src="https://github.com/akshay23sept/Simulation-approach-in-C-and-Python/blob/master/images/active_particles.gif" align="right" style="max-width:50%;"></a> <code>tmpmail</code> </p>
This repo contains general pupose Lattice Boltzmann code and has been in implemented in the research performed by me entitled Dynamics of diatoms in turbulent flow.
In this research we focused on diatoms which are unicellular microorganism deprived of swimming capabilities. We model diatoms as non spherical particles elongated and thin, modeled as a particle undergoing the effect of drag. These particles were placed in a homogeneous and isotropic turbulent flow (direct numerical simulation, DNS), in which a passive scalar was also simulated. The passive scalar fields represented the nutritive salt necessary for the growth of diatoms. Numerical simulation targeted to consider the rate of the encounter between planktonic organism and nutrients, under the effect of turbulence. We also studied the influence of the nonspherical shape of the particle on the encounter rate.
