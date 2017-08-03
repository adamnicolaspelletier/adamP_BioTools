# adamP_BioTools
Collection of scripts to generate synthetic promoters recognized by specific Transcription Factors

### Author: Adam-Nicolas Pelletier
### Github: https://github.com/adamnicolaspelletier/adamP_BioTools.git

## Table of Contents

- [Requirements](#requirements)
- [Installation](#installation)
- [Information](#information)
- [Usage](#usage)
- [In Development](#in-development)
- [Known Bugs](#known-bugs)
- [Support](#support)
- [Contributing](#contributing)



## Requirements

* Python 2.7+

* Python Libraries :

  1. Pandas (+ Numpy) 0.20.1+
  2. BioPython 1.69+





## Installation

The easiest installation method is through PyPi. It will install the package directly with other packages, after typing the following command:

```sh
pip install adamP_BioTools

```

It can also be downloaded to your project directory from GitHub as a module, or clone it on the command line using the following command:

```sh
git clone git://github.com/adamnicolaspelletier/adamP_BioTools.git

```

## Information

During my computational biology analysis and engineering, I have come to develop several simple functions that were reused constantly. I have organized such functions into a simple package,  which can be imported as needed. These functions range from simple DNA string reverse complementation, DNA string to numpy array conversion, to PSSM alignment with DNA motifs.

This significantly reduces overhead in scripts, allowing for more concise and reproducible code. 
This is not meant to be used as an organized package for specific purpose (graphics, or dataframe manipulation): it is a personal collection of functions. As more are added over time, the package might be split into several based on theme and utility. Thus, I highly suggest for users to verify changes before upgrading. 


## Usage

The package has been split into 2 modules: dna_tools.py and os_handling.py
The former has several functions involved in the treatment of biological data and structures. 
The latter is used to verify file validity, output name redundance.

Each function has different arguments and takes different input and output. 

To list all functions and, you can first import the module, then ask for help:

```sh
from adamP_BioTools import dna_tools
from adamP_BioTools import os_handling

help(dna_tools)

```

However, when imported this way, each function must use dna_tools as a prefix to each function, which can be cumbersome. 

The best way to get help for a specific function is to call for the help command in a Python console after importing either the whole module, or specific functions.

```sh
from adamP_BioTools.dna_tools import *    # whole module
from adamP_BioTools.dna_tools import topseq   #only topseq function
from adamP_BioTools.os_handling import path_validity

help(topseq)

```



## In Development

Nothing specific at this moment, but redundant functions tend to be added here over time to avoid duplication. 


## Known Bugs

No bugs are currently known.

## Support

Please [open an issue](https://github.com/adamnicolaspelletier/adamP_BioTools.git/issues/new) for support.


## Contributing

Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/adamnicolaspelletier/adamP_BioTools/compare/).
