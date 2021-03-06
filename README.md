[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3891992.svg)](https://doi.org/10.5281/zenodo.3891992)

# MMS SITL Ground Loop: Notebooks to Train and Run the GLS-MP Model
This project is part of the [MMS mission](https://lasp.colorado.edu/mms/sdc/public/) at the University of Colorado-Boulder's [Laboratory for Atmospheric and Space Physics](http://lasp.colorado.edu/home/) and the University of New Hampshire's [Space Science Center](https://eos.unh.edu/space-science-center). 

## Project Intro/Objective
The GLS-MP software is designed to provide automated magnetopause crossing selection suggestions for the SITL selection team. The software uses a [TensorFlow Keras](https://www.tensorflow.org/guide/keras) [LSTM (long short term memory) neural network](https://en.wikipedia.org/wiki/Long_short-term_memory) trained on previous magnetopause selections in order to generate novel suggested crossing selection windows.

The software is fully integrated into the SDC and SITL workflow, providing suggested magnetopause crossings in near real-time.

### Authors
* Colin Small, [University of New Hampshire Department of Computer Science](https://ceps.unh.edu/computer-science)
* [Matthew R. Argall](https://mypages.unh.edu/argallmr/bio), [University of New Hampshire Space Science Center](https://eos.unh.edu/space-science-center)
* [Marek Petrik](https://ceps.unh.edu/person/marek-petrik), [University of New Hampshire Department of Computer Science](https://ceps.unh.edu/computer-science)

## Notebooks

This project contains two notebooks, both of which we suggest you open with Google Colab:

* [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/colinrsmall/GLS-MP/blob/master/Run_Model.ipynb) **Run Model** - This notebook is used to run the GLS-MP model to generate magnetopause selections. 

* [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/colinrsmall/GLS-MP/blob/master/Model_Development.ipynb) **Model Development** - This notebook walks the reader through the training of the GLS MP model, and was the notebook used to train the original version of the model currently in use at the SDC. 

## See Also:

* [mms_sitl_ground_loop](https://github.com/argallmr/mms_sitl_ground_loop) - This repository contains notebooks used to generate figures specific to **Argall, Small, et al. (2020)**, the paper describing this model and its implementation at the SDC.

* [PyMMS](https://github.com/argallmr/pymms) - This repository contains tools and scripts for accessing data at the SDC, from MMS mission data to GLS-MP generated selections.

* [mp-dl-unh](https://github.com/colinrsmall/mp-dl-unh) - This repository contains tools and scripts specifically for running the GLS-MP model at the SDC.

## Attribution

If you reference GLS-MP in your academic projects in the context of its deployment at the SDC, please cite **Argall, Small, et al. (2020)**. To cite the library in general, you could use this BibTeX entry:

```
@software{Small:2020,
author = {Small, C. R. and Argall, M. R. and Petrik, M.},
doi = {10.5281/zenodo.3891992},
month = {jun},
publisher = {Zenodo},
title = {{MMS SITL Ground Loop: Notebooks to Train and Run the GLS-MP Model}},
url = {https://doi.org/10.5281/zenodo.3891991},
year = {2020}
}
```
