# Simulation-approach-in-C
## A <code>Lattice-Boltzmann method (LBM)</code> based approach to study Eulerian-Lagrangian fluid dynamics
![alt text](https://github.com/akshay23sept/Simulation-approach-in-C-and-Python/blob/master/images/example.png)
<h2><a id="user-content-introduction" class="anchor" aria-hidden="true" href="https://github.com/akshay23sept/Simulation-approach-in-C-and-Pythonintroduction"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Introduction:</h2>
<div><pre><span>.</span>
###<p>A general purpose <em>Lattice-Boltzmann</em> code for fluid-dynamics simulations. The code includes :</p>###
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

<h2><a id="user-content-downloadclone" class="anchor" aria-hidden="true" href="https://github.com/akshay23sept/akshay23sept.github.io#downloadclone"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><a id="user-content-requirements" href="https://github.com/akshay23sept/akshay23sept.github.io#Downlaod"></a>Download/Clone:</h2>
<ol>
<p><code>$ git clone https://github.com/akshay23sept/akshay23sept.github.io</code></p>
</ol>

<h2><a id="user-content-directory-structure" class="anchor" aria-hidden="true" href="https://github.com/akshay23sept/akshay23sept.github.io#directory-structure"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><a id="user-content-directory-structure" href="https://github.com/aakash30jan/LatexToWebpage#directory-structure"></a>Directory Structure:</h2>
<div><pre><span>.</span>
├── CV
│&nbsp;&nbsp; ├── AkshayAnand.jpg
├── backup
│&nbsp;&nbsp; ├── several version of index files
│&nbsp;&nbsp; │&nbsp;&nbsp; └── [ALL moderncv documnetclass files]
├── index.html
├── favicon
│&nbsp;&nbsp; ├── several favicon images
├── conferences
│&nbsp;&nbsp; ├── several conference papers
├── presentation
│&nbsp;&nbsp; ├── several presentation images
├── LICENSE
├── README.md
└── website
    ├── <span>&lt;</span>PUT ALL PROJECT IMAGES HERE<span>&gt;</span>
    └── js
        └── scramble.js</pre></div>
<h2><a id="user-content-prerequisite" class="anchor" aria-hidden="true" href="https://github.com/akshay23sept/akshay23sept.github.io#prerequisite"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><a id="user-content-requirements" href="https://github.com/akshay23sept/akshay23sept.github.io#Prerequisite"></a>Prerequisite:</h2>
<ol>
<li>Python 2.7 or above</li>
<li>Latex essentials: texstudio, texlive-latex-extra, overleaf, texlive-fonts-recommended</li>
</ol>
<h2><a id="user-content-downloadclone" class="anchor" aria-hidden="true" href="https://github.com/akshay23sept/akshay23sept.github.io#downloadclone"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><a id="user-content-requirements" href="https://github.com/akshay23sept/akshay23sept.github.io#Downlaod"></a>Download/Clone:</h2>
<ol>
<p><code>$ git clone https://github.com/akshay23sept/akshay23sept.github.io</code></p>
</ol>
<h2><a id="user-content-exploiting-the-code" class="anchor" aria-hidden="true" href="https://github.com/akshay23sept/akshay23sept.github.io#exploiting-the-code"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><a id="user-content-using-the-code" href="https://github.com/akshay23sept/akshay23sept.github.io#exploiting-the-code"></a>Exploiting the code:</h2>
<ol>
<li><code>Update</code> the <code>index.html</code> file with your relevant information.</li>
<li>Your updated webpage can be checked with <code>firefox index.html</code>.</li>
<li>You may now upload the webpage to your favourite hosting service.</li>
</ol>


<h2><a id="user-content-introduction" class="anchor" aria-hidden="true" href="https://github.com/akshay23sept/Simulation-approach-in-C-and-Python#Prerequisite:"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Prerequisite:</h2>
<ol>
<li>Python 2.7 or above</li>
<li>C++</li>
<li>HDF5</li> 
<li>MPI</li>
<li>CMake</li>
</ol>
<h2><a id="user-content-introduction" class="anchor" aria-hidden="true" href="https://github.com/akshay23sept/Simulation-approach-in-C-and-Python#Exploiting the codes:"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Exploiting the codes:</h2>
<ol>
Download or clone the codes using:
<p><code>$ git clone https://github.com/akshay23sept/Simulation-approach-in-C-and-Python</code></p>
Please check the ![wiki page](https://github.com/akshay23sept/Simulation-approach-in-C-and-Python/blob/master/images/example.png) for more information
</ol>
<h2><a id="user-content-downloadclone" class="anchor" aria-hidden="true" href="https://github.com/akshay23sept/akshay23sept.github.io#downloadclone"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><a id="user-content-requirements" href="https://github.com/akshay23sept/akshay23sept.github.io#Downlaod"></a>Download/Clone:</h2>
<ol>
<p><code>$ git clone https://github.com/akshay23sept/akshay23sept.github.io</code></p>
</ol>
<h2><a id="user-content-introduction" class="anchor" aria-hidden="true" href="https://github.com/akshay23sept/Simulation-approach-in-C-and-Python#Issues:"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Issues:</h2>
<ol>
Feel free to raise an issue at <a href="https://github.com/akshay23sept/Simulation-approach-in-C-and  Python">https://github.com/akshay23sept/Simulation-approach-in-C-and-Python</a>
</ol>
</h1>
<div class="Box-body px-5 pb-5">
<article class="markdown-body entry-content container-lg" itemprop="text"><h1><a id="user-content-personal-website" class="anchor" aria-hidden="true" href="https://github.com/akshay23sept/Simulation-approach-in-C-and-Python#introduction"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 Introduction:</h1>
<p>A general purpose Lattice-Boltzmann code for fluid-dynamics simulations.
<br></p>
<h2><a id="user-content-directory-structure" class="anchor" aria-hidden="true" href="https://github.com/akshay23sept/Simulation-approach-in-C-and-Python#directory-structure"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><a id="user-content-directory-structure" href="https://github.com/akshay23sept/Simulation-approach-in-C-and-Python#code-includes"></a>Code Includes:</h2>
