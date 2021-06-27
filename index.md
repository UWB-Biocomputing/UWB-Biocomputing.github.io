todo: make this


[![DOI](https://zenodo.org/badge/6034062.svg)](https://zenodo.org/badge/latestdoi/6034062)

## The Graphitti Project

The original idea behind the Graphitti Project is to develop a toolkit/software architecture to ease creating high-performance network simulators. It is now composed of two parts Graphitti (the simulator) and Workbench (a simulation and data/software provenance tool). So, we now say that Graphitti+Workbench focuses on enabling **high-performance/high-quality** neural simulation.

### [Graphitti](https://uwb-biocomputing.github.io/Graphitti/)

A project to facilitate construction of high-performance neural simulations.

#### Key features:
- Its target audience are researchers who need higher performance than that made available by general-purpose simulators, those that use Python, etc. and who are therefore considering writing their own simulation code in C/C++.
- Its target application is large scale and long duration neural simulations.
- It provides a C++ programming interface that focuses new coding just on the core implementation of neuron, synapse, etc. state updates.
- It assumes that an investigator will first want to implement small and/or short duration simulations that run as a single thread on a CPU, to provide validation data to increase confidence in result validity (this is part of the "high quality" theme).
- It provides a programming interface to minimize code changes needed to port the simulation to single or multiple GPUs. In effect, we've already optimized the simulator for GPUs (this addresses the "high performance" aspect).

### [Workbench](https://UWB-Biocomputing.github.io/WorkBench/)

Software and data provenance management platform for simulations of dissociated cortical cultures.

#### Key features:
- A Java-based Workbench that allows the investigator to download, build, and run the simulator.
- Captures all software and data provenance information so that later, the investigator can compare different results generated at different times and see how they differ in terms of not only their input parameters but also their simulator versions. 
- Helps one to determine whether two simulations are comparable, whether one or more are invalid due to simulator bugs, etc. (This also connects to the idea of "high quality".)



### Examples [under construction]

### [Lab Publication](https://uwb-biocomputing.github.io/Graphitti/docs/BGDocs/lab-publication.md) 

### [Acknowledgements](https://uwb-biocomputing.github.io/Graphitti/docs/BGDocs/acknowledgements.md)

---------
### Multiple simulation architectures:

- Single-threaded on general-purpose CPU
- GPU-accelerated using NVIDIA's CUDA libraries
- Multi-cluster (using multiple CPU cores and/or multiple GPUs) — *under development*
- GPU-accelerated using OpenCL — *planned*
- Multi-threading using OpenMP — *planned*

### Supported operating systems:

- GNU Linux

### Graphitti Resources:

- [Graphitti Forum]([https://groups.google.com/forum/#!forum/uwb-graphitti](https://groups.google.com/forum/#!forum/uwb-braingrid)): A place where Graphitti artists can communicate and collaborate. Click the button "Apply to join this group" to join!
- [Git Crash Course](https://github.com/UWB-Biocomputing/BrainGrid/wiki/Git-Crash-Course)
- [Linux Crash Course](https://github.com/UWB-Biocomputing/BrainGrid/wiki/Linux-Crash-Course)


### Doxygen 

[Visit Doxygen Generated Documentation](docs/Doxygen/html/index.html)
[Visit Doxygen Generated Documentation w/o docs root](Doxygen/html/index.html)
