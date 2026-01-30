# Refractive Compensating Smart Window Simulations

This repository contains the simulation models and design files for the **Double Layer Corner Cube (DLCC)** structure, a novel optofluidic smart glass designed to maintain transparency even with imperfect refractive index matching.

## Research Overview

Traditional smart windows based on corner cube geometry often suffer from "tri-refractions" and loss of image resolution if the fluid used for transparency does not perfectly match the refractive index of the building material. This project introduces the **DLCC structure**, which uses an additional layer of corner cubes to correct the path of light rays, ensuring they continue in a straight path regardless of slight index mismatches.

## Software & Requirements

The following software tools were used for the design, simulation, and analysis of the refractive compensating structures:

 
**AutoCAD 3D**: Used for the initial 3D modeling of the DLCC and corner cube clusters.


  
**LightTools**: Primary ray-tracing software used for testing retro-reflectivity, image resolution, and the impact of fabrication tolerances.


  
**MATLAB**: Utilized for extracting RGB matrices from complex images and calculating tristimulus values for perceived color analysis.



## Simulation Methodology

The repository is structured to replicate the three main phases of testing described in the paper:

### 1. Preliminary Ray Fan Tests

Simulations aimed at observing basic ray behavior through the DLCC vs. standard Corner Cube boxes.


**Materials**: PMMA (n=1.49) and 2,2'-Thiodiethanol (n=1.52).



### 2. Complex Image & Viewer Distance Analysis

Tests that evaluate image resolution from a viewer's perspective at varying distances (e.g., 2cm, 20cm).


**Technique**: Overlapping three separate RGB sources (650nm, 550nm, 450nm) weighted by blackbody temperature to create "True Color" results.



### 3. Fabrication Tolerance Modeling

Simulations that incorporate a **0.1mm CNC machining tolerance** (rounding of internal corners) to investigate the mismatch between ideal simulations and physical prototypes.

## Core Equations

The simulations utilize **Fresnel coefficients** to model reflectance and transmittance at normal incidence:

$$ R_{F} = \left(\frac{n_1 - n_2}{n_1 + n_2}\right)^2 $$
 
Where $$R_F$$ is the power reflectance and $$n_x$$ represents the refractive indexes of the media.

## Citation

If you use these simulation models or the DLCC design in your research, please cite the original paper:

```bibtex
@inproceedings{barbosa_optofluidic_2025,
	location = {San Diego, United States},
	title = {Optofluidic smart glass with refractive-compensating structure allowing transparency with refractive index mismatch},
	isbn = {978-1-5106-9098-1 978-1-5106-9099-8},
	url = {https://www.spiedigitallibrary.org/conference-proceedings-of-spie/13595/3062607/Optofluidic-smart-glass-with-refractive-compensating-structure-allowing-transparency-with/10.1117/12.3062607.full},
	doi = {10.1117/12.3062607},
    note = "[doi:10.1117/12.3062607]",
	eventtitle = {Novel Optical Systems, Methods, and Applications {XXVIII}},
	pages = {33},
	booktitle = {Novel Optical Systems, Methods, and Applications {XXVIII}},
	publisher = {{SPIE}},
	author = {Barbosa, Priscila Maria and Goossen, Keith W.},
	editor = {Hahlweg, Cornelius F. and Mulley, Joseph R.},
	urldate = {2025-11-06},
	date = {2025-09-18},

```

## Usage Restrictions & Intellectual Property
**All Rights Reserved.**

This repository contains the simulations and design files for the DLCC smart window structure as described in the published research. 

**Unauthorized use, reproduction, or modification of the files and the associated 3D models is strictly prohibited.** These files are provided solely for the purpose of academic peer review and verification of results. It may not be:
* Used to create derivative works.
* Used for any commercial or industrial applications.
* Redistributed in any form without express written consent from the authors and the University of Delaware.

For licensing inquiries or permission to use these models, please contact the author.

## Contact

**Priscila M. Barbosa** - [pbarbosa@udel.edu](mailto:pbarbosa@udel.edu)





