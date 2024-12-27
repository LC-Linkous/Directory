# Directory of Repository Projects and Related Publications

Publications and research can be found on my [Google Scholar](https://scholar.google.com/citations?user=UHCDo0MAAAAJ&hl=en&oi=ao) and [ResearchGate](https://www.researchgate.net/profile/Lauren-Linkous) pages
<br>
<br>
Interested in collaboration? Reach out to me on [LinkedIn](https://www.linkedin.com/in/lauren-linkous)!


Repositories are grouped together by topic, so expect some duplicate links. See individual repositories for a list of associated sources (papers, libraries, repositories), and associated publications.


## Table of contents
* [Ongoing Projects](#ongoing-projects)
* [AntennaCAT](#antennacat)
* [Optimizers and Surrogate Models](#optimizers-and-surrogate-models)
* [Objective Function Benchmark Suite](#objective-function-benchmark-suite)
* [AntennaCalculator](#antennacalculator)
* [Papers with Repositories and Tutorials](#papers-with-repositories-and-tutorials)
* [Tutorials](#tutorials)
* [Small Project Examples](#small-project-examples)
  * [Machine Learning](#machine-learning)
  * [GUI Examples](#gui-examples)
    * [Realtime Graphing](#realtime-graphing)
    * [Visual Machine Learning ](#visual-machine-learning)
    * [General References](#general-references)
* [Licensing](#licensing)
* [Publications](#publications)
* [FAQs](#faqs)



## Ongoing Projects
Primary ongoing projects:

* The [AntennaCalculationAutotuningTool](https://github.com/LC-Linkous/AntennaCalculationAutotuningTool), "AntennaCAT", is an ongoing open-source project to make antenna design easier by automating the design, calculation, scripting, and tuning of antennas created in several common simulation software. It is designed to be compatible with multiple EM simulation software.   

* Collaborative effort forked from [Dollarhyde's](https://github.com/Dollarhyde/AntennaCalculator), the [Antenna Calculator](https://github.com/LC-Linkous/AntennaCalculator) is the internal calculator for common topologies in the AntennaCAT project. Designs are being updated as they're tested/validated.

* Project documentation and [tutorial series](#tutorials)



## AntennaCAT

<p align="center">
 <img src="https://github.com/LC-Linkous/AntennaCalculationAutotuningTool/blob/main/media/antennaCAT-icons/transparent-antennaCAT-logo.png" height="300" >
</p>


Antenna Calculation and Autotuning (AntennaCAT) is a comprehensive implementation of machine learning to automate, evaluate, and optimize the antenna design process using EM simulation software. It utilizes a combined antenna designer and internal calculator to accelerate the CAD construction and EM simulation of several common topologies, while eliminating model disparity for automated data collection.


For more information and current project status, refer to the [AntennaCAT main repository](https://github.com/LC-Linkous/AntennaCalculationAutotuningTool/) and the [Wiki documentation](https://github.com/LC-Linkous/AntennaCalculationAutotuningTool/wiki)


### Related Repositories 

See the following sections:
* [Optimizers and Surrogate Models](#optimizers-and-surrogate-models)
* [AntennaCalculator](#antennacalculator)



## Optimizers and Surrogate Models
---

The following are a collection of state-machine-based optimizers compatible with the AntennaCAT project. Most, if not all, have been integrated into the main AntennaCAT project. These optimizers are functional stand alone for testing and publication transparency. Some have been incorporated into other research projects or publications, which are noted on the individual README pages.

All optimizers and surrogate model examples work on state machine logic in order to incorporate substituting simulation for the objective functions in AntennaCAT. 


**Summary of Optimizers**

| Base Optimizer | Alternate Version | Quantum-Inspired Optimizer | Surrogate Model Version |
| ------------- | ------------- | ------------- |------------- |
| [pso_python](https://github.com/LC-Linkous/pso_python) | [pso_basic](https://github.com/LC-Linkous/pso_python/tree/pso_basic) | [pso_quantum](https://github.com/LC-Linkous/pso_python/tree/pso_quantum)  | |
| [cat_swarm_python](https://github.com/LC-Linkous/cat_swarm_python) | [sand_cat_python](https://github.com/LC-Linkous/cat_swarm_python/tree/sand_cat_python)| [cat_swarm_quantum](https://github.com/LC-Linkous/cat_swarm_python/tree/cat_swarm_quantum) | |
| [chicken_swarm_python](https://github.com/LC-Linkous/chicken_swarm_python) | [2015 improved chicken swarm](https://github.com/LC-Linkous/chicken_swarm_python/tree/improved_chicken_swarm) | [chicken_swarm_quantum](https://github.com/LC-Linkous/chicken_swarm_python/tree/chicken_swarm_quantum)  | |
| [sweep_python](https://github.com/LC-Linkous/sweep_python)  | *alternates in base repo | -  | - |
| [bayesian optimization_python](https://github.com/LC-Linkous/bayesian_optimization_python)  | -| - | *interchangeable surrogate models <br> included in base repo |
| [multi_glods_python](https://github.com/LC-Linkous/multi_glods_python)| - | - | |

**Objective Functions**


The [Objective Function Test Suite](https://github.com/LC-Linkous/objective_function_suite) used to generate training data


### **Repository Details**


 * J. Lundquist, L. Linkous (2024) pso_python (Version 1.0) [source code] https://github.com/jonathan46000/pso_python
    1) [pso_python](https://github.com/jonathan46000/pso_python) by [jonathan46000](https://github.com/jonathan46000)
    2) the main branch with the [adaptive timestep PSO optimizer](https://github.com/jonathan46000/pso_python)  by [jonathan46000](https://github.com/jonathan46000)
    3) the [pso_basic branch](https://github.com/jonathan46000/pso_python/tree/pso_basic) without the timestep, for a baseline comparison by [LC-Linkous](https://github.com/LC-Linkous)
    4) [LC-Linkous' development fork](https://github.com/LC-Linkous/pso_python)
       
* L. Linkous, J. Lundquist (2024) sweep_python (Version 1.0) [source code] (https://github.com/LC-Linkous/sweep_python)
   1) [sweep](https://github.com/LC-Linkous/sweep_python) by [LC-Linkous](https://github.com/LC-Linkous), a basic sweep optimization example compatible with AntennaCAT. Features grid search and random search.
  
* L. Linkous, J. Lundquist (2024) cat_swarm_python (Version 1.0) [source code] (https://github.com/LC-Linkous/cat_swarm_python)
    1) [cat_swarm_python](https://github.com/LC-Linkous/cat_swarm_python)  by [LC-Linkous](https://github.com/LC-Linkous),
    2) the main branch with [traditional cat swarm optimizer](https://github.com/LC-Linkous/cat_swarm_python/tree/main)  by [LC-Linkous](https://github.com/LC-Linkous)
    3) the [sand cat swarm branch](https://github.com/LC-Linkous/cat_swarm_python/tree/sand_cat_python)  by [LC-Linkous](https://github.com/LC-Linkous)
    4) the [quantum inspired cat swarm branch](https://github.com/LC-Linkous/cat_swarm_python/tree/cat_swarm_quantum) with a numpy-based quantum inspired (probabilistic) approach  by [LC-Linkous](https://github.com/LC-Linkous)
  
* L. Linkous, J. Lundquist (2024) chicken_swarm_python (Version 1.0) [source code] (https://github.com/LC-Linkous/chicken_swarm_python)
    1) [chicken_swarm_python](https://github.com/LC-Linkous/chicken_swarm_python)  by [LC-Linkous](https://github.com/LC-Linkous)
    2) the main branch with [traditional chicken swarm optimizer](https://github.com/LC-Linkous/chicken_swarm_python) by [LC-Linkous](https://github.com/LC-Linkous)
    3) the [chicken_swarm_quantum branch](https://github.com/LC-Linkous/chicken_swarm_python/tree/chicken_swarm_quantum) with a very simple, numpy-based quantum inspired approach by [LC-Linkous](https://github.com/LC-Linkous) 
  
* J. Lundquist, L. Linkous (2023) multi_glods_python (Version 1.0) [source code] https://github.com/jonathan46000/multi_glods_python
  1) [multi_glods_python](https://github.com/jonathan46000/multi_glods_python) by [jonathan46000](https://github.com/jonathan46000)
  2) The main branch and fork are now compatible with AntennaCAT

* L. Linkous, (LC-Linkous) (2024) Objective Function Suite (Version 1.0) https://github.com/LC-Linkous/objective_function_suite
   1) [Objective Function Test Suite](https://github.com/LC-Linkous/objective_function_suite)
   2) 50+ single, multi, and constrained objective functions compatible with the optimizer collection


## Objective Function Benchmark Suite
--- 

This repository contains a comprehensive benchmarking framework for evaluating the performance of various optimizers in hyperparameter tuning tasks, and the ability to collect data on optimizer performance for machine learning tasks. Additional objective functions updated periodically.

It contains:
1)  **Objective Function Library**: is a collection of 50+ single objective functions, multi objective functions, and constrained objective functions formatted with work with the optimizer collection in the [Optimizers and Surrogate Models](#Optimizers and Surrogate Models) section
2)  **Optimizer Suite**: The optimizers included in this project are static versions of the optimizers integrated into the [AntennaCAT](#https://github.com/LC-Linkous/AntennaCalculationAutotuningTool) software suite.
3) **Optimizer Performance Data Collection**: Scripts for replicating the data collection method used to develop the AntennaCAT project.  


### **Repository Details**

* L. Linkous, (LC-Linkous) (2024) Objective Function Suite (Version 1.0) https://github.com/LC-Linkous/objective_function_suite
   1) [Objective Function Test Suite](https://github.com/LC-Linkous/objective_function_suite)
   2) Contains the objective function library, a static version of the optimizer suite (for compatibility), and scripts used in data collection. 
    

## AntennaCalculator
---

<p align="center">
        <img src="https://github.com/LC-Linkous/AntennaCalculator/blob/GUI/media/patch_preview.png" alt="screenshot of the GUI featuring the output of calculating the rectangular patch antenna" height="250">    </p>
   <p align="center">Calculated and Previewed Microstrip Rectangular Patch Antenna</p>


A forked GUI branch of [Dollarhyde's](https://github.com/Dollarhyde) [CLI-based AntennaCalculator](https://github.com/Dollarhyde/AntennaCalculator). This branch is a simplified version of how the AntennaCalculator is integrated into [LC-Linkous'](https://github.com/LC-Linkous) [AntennaCAT project](https://github.com/LC-Linkous/AntennaCalculationAutotuningTool). It features some matplotlib-based graphics to help visualize the antenna topologies based on user inputs. 

The calculator features the following topologies:
* Rectangular patch antenna, probe and microstrip versions
* Quarter Wave Monopole
* Half Wave Dipole

### **Repository Details**
---
* E. Karincic, (Dollarhyde) (2022) Antenna Calculator (Version 2.0) [source code]. https://github.com/Dollarhyde/AntennaCalculator
  1) [Antenna Calculator](https://github.com/Dollarhyde/AntennaCalculator) by [Dollarhyde](https://github.com/Dollarhyde)
  2) The original, [command-line based AntennaCalculator](https://github.com/Dollarhyde/AntennaCalculator)
  3) The python-based [GUI wrapper of the AntennaCalculator](https://github.com/LC-Linkous/AntennaCalculator/tree/GUI)
  4) [LC-Linkous' development fork](https://github.com/LC-Linkous/AntennaCalculator)



## Papers with Repositories and Tutorials
--- 

### _Machine Learning Assisted Hyperparameter Tuning for Optimization_
**Paper**:

L. Linkous, J. Lundquist, M. Suche and E. Topsakal, "Machine Learning Assisted Hyperparameter Tuning for Optimization," 2024 IEEE INC-USNC-URSI Radio Science Meeting (Joint with AP-S Symposium), Florence, Italy, 2024, pp. 107-108, doi: 10.23919/INC-USNC-URSI61303.2024.10632482.

**Repository**:

* L. Linkous (LC-Linkous) (2023) PSO_datacollection (Version 1.0) [source code]. https://github.com/LC-Linkous/PSO_datacollection
  1) [Antenna Calculator](https://github.com/LC-Linkous/PSO_datacollection) by [LC-Linkous](https://github.com/LC-Linkous)
  2) This is the original repository linked in publication, but it has since been renamed as other presentations have been added

* L. Linkous (LC-Linkous) (2023) 2024-APS-URSI-3323 (Version 2.0) [source code]. https://github.com/LC-Linkous/2024-APS-URSI-3323
  1) [2024-APS-URSI-3323](https://github.com/LC-Linkous/2024-APS-URSI-3323)  by [LC-Linkous](https://github.com/LC-Linkous)
  2) Repository hosting data and select machine learning examples from publication ["Machine Learning Assisted Hyperparameter Tuning for Optimization"](https://ieeexplore.ieee.org/abstract/document/10632482)

### _Machine Learning Assisted Optimization Methods for Automated Antenna Design_
**Paper**:

L. Linkous and E. Topsakal, "Machine Learning Assisted Optimization Methods for Automated Antenna Design," 2024 United States National Committee of URSI National Radio Science Meeting (USNC-URSI NRSM), Boulder, CO, USA, 2024, pp. 377-378, doi: 10.23919/USNC-URSINRSM60317.2024.10464597. [Online:] https://ieeexplore.ieee.org/abstract/document/10464597

**Repository**:

* L. Linkous (LC-Linkous) (2023) 2024-URSI-NRSM-1265 (Version 1.0) [source code]. https://github.com/LC-Linkous/2024-URSI-NRSM-1265
  1) [2024-URSI-NRSM-1265](https://github.com/LC-Linkous/2024-URSI-NRSM-1265)  by [LC-Linkous](https://github.com/LC-Linkous)
  2) Repository for publication ["Machine Learning Assisted Optimization Methods for Automated Antenna Design"](https://ieeexplore.ieee.org/abstract/document/10464597)
  3) Features 5 tutorials using Jupyter Notebook to process and analyze a subset of simulation data for patch antennas


### _Patch Antenna Calculations and Fabrication Made Simple for Cyber Security Research_
**Paper**:

E. Karincic, E. Topsakal, and L. Linkous.  "Patch Antenna Calculations and Fabrication Made Simple for Cyber Security Research,"  2023 ASEE Annual Conference & Exposition, Baltimore , Maryland, 2023, June.  ASEE Conferences, 2023. [Online:] https://peer.asee.org/43974 

**Repository**:

* E. Karincic, (Dollarhyde) (2022) Antenna Calculator (Version 2.0) [source code]. https://github.com/Dollarhyde/AntennaCalculator
  1) [Antenna Calculator](https://github.com/Dollarhyde/AntennaCalculator) by [Dollarhyde](https://github.com/Dollarhyde)
  2) The original, [command-line based AntennaCalculator](https://github.com/Dollarhyde/AntennaCalculator)
  3) The python-based [GUI wrapper of the AntennaCalculator](https://github.com/LC-Linkous/AntennaCalculator/tree/GUI)
  4) [LC-Linkous' development fork](https://github.com/LC-Linkous/AntennaCalculator)


## Tutorials
---

| Project  |  Need Anything Not in the Code Repo?       |       Tutorial Links       |
|-----------|--------------------------------------------|----------------------------|
| [AntennaCAT](https://github.com/LC-Linkous/AntennaCalculationAutotuningTool) | Needs EM simulation software license | <ul><li>[Main Wiki](https://github.com/LC-Linkous/AntennaCalculationAutotuningTool/wiki)</li><li>[Guides and Tutorials page](https://github.com/LC-Linkous/AntennaCalculationAutotuningTool/wiki/Guides-and-Tutorials)</li></ul> |
| [JTAGenum project fork](https://github.com/LC-Linkous/JTAGenum)     | Hardware reqs. in the README  |  <ul><li>[Forked Project Wiki](https://github.com/LC-Linkous/JTAGenum/wiki)</li><li>pages in the wiki associated with this repository. TODO</li></ul>       |
|            |                 |         |
|            |                 |         |
|            |                 |         |



## Small Project Examples
---

### **Machine Learning**

* A [WXPython version](https://github.com/LC-Linkous/Example_Genetic-Algorithm-Drawing) of [Samuel Hinton's Genetic Algorithm tutorials](https://cosmiccoding.com.au/tutorials/genetic_part_one/)

### **GUI Examples**
#### Realtime Graphing

* A [TK GUI example](https://github.com/LC-Linkous/Example_Matplotlib-Tkinter) of realtime plotting. Mentioned previously on an old project blog, the page will be reposted.

* A [WXPython GUI example](https://github.com/LC-Linkous/Example_wxPython-Pages) of realtime plotting. Mentioned previously on an old project blog, the page will be reposted.

#### Visual Machine Learning 
* A [WXPython version](https://github.com/LC-Linkous/Example_Genetic-Algorithm-Drawing) of [Samuel Hinton's Genetic Algorithm tutorials](https://cosmiccoding.com.au/tutorials/genetic_part_one/)

#### General References
* A [WXPython Multi-page example](https://github.com/LC-Linkous/Example_wxPython-Pages)




## Licensing
---

The source code linked in this documentation has been released under a variety of licenses, some as requested from their original source publication, so refer to the individual READMEs of each project (and the LICENSE file) for the most accurate information.


## Publications
---


* L. Linkous, “Machine Learning Assisted Optimization for Calculation and Automated Tuning of Antennas,” VCU Scholars Compass, 2024. https://scholarscompass.vcu.edu/etd/7841/ (accessed Oct. 21, 2024).

* L. Linkous, J. Lundquist, M. Suche and E. Topsakal, "Machine Learning Assisted Hyperparameter Tuning for Optimization," 2024 IEEE INC-USNC-URSI Radio Science Meeting (Joint with AP-S Symposium), Florence, Italy, 2024, pp. 107-108, doi: 10.23919/INC-USNC-URSI61303.2024.10632482. [Online:] https://ieeexplore.ieee.org/abstract/document/10632482

* L. Linkous and E. Topsakal, "Machine Learning Assisted Optimization Methods for Automated Antenna Design," 2024 United States National Committee of URSI National Radio Science Meeting (USNC-URSI NRSM), Boulder, CO, USA, 2024, pp. 377-378, doi: 10.23919/USNC-URSINRSM60317.2024.10464597. [Online:] https://ieeexplore.ieee.org/abstract/document/10464597

* L. Linkous, J. Lundquist and E. Topsakal, "AntennaCAT: Automated Antenna Design and Tuning Tool," 2023 IEEE USNC-URSI Radio Science Meeting (Joint with AP-S Symposium), Portland, OR, USA, 2023, pp. 89-90, doi: 10.23919/USNC-URSI54200.2023.10289238.  [Online:] https://ieeexplore.ieee.org/abstract/document/10289238

* E. Karincic, E. Topsakal, and L. Linkous.  "Patch Antenna Calculations and Fabrication Made Simple for Cyber Security Research,"  2023 ASEE Annual Conference & Exposition, Baltimore , Maryland, 2023, June.  ASEE Conferences, 2023. [Online:] https://peer.asee.org/43974 

* L. Linkous, E. Karincic, J. Lundquist and E. Topsakal, "Automated Antenna Calculation, Design and Tuning Tool for HFSS," 2023 United States National Committee of URSI National Radio Science Meeting (USNC-URSI NRSM), Boulder, CO, USA, 2023, pp. 229-230, doi: 10.23919/USNC-URSINRSM57470.2023.10043119.  [Online:] https://ieeexplore.ieee.org/abstract/document/10043119



## FAQs
--- 

### When will the AntennaCAT source code be public?
Roughly Fall/Winter 2024. The AntennaCAT project is my PhD dissertation. Related code (such as the optimizers and sample data/tutorials) are being released periodically, but the main AntennaCAT software suite will be released after my dissertation defense.


### The hyperlinks to your repos are broken.
  e.g., these: L. Linkous, (LC-Linkous) (2022) AntennaCAT (Version 2024.0) [source code] https://github.com/LC-Linkous/AntennaCalculationAutotuningTool
  
  They're in IEEE format. I'm lazy and ctrl+C ctrl+V these into my references when I'm writing a paper.

  
  e.g, others.
  
  Let me know and I'll update them. Some repos have been renamed, or code moved, as projects have evolved to keep things readable. I try my best to update all the links, but occasionally miss one.

### Have you heard of spell check?
  Yes. Soemtiems I can even ues it.

