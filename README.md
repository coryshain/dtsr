# Deconvolutional time series regression (DTSR)
DTSR is a regression technique for modeling temporally diffuse effects (Shain & Schuler, 2018).

This repository contains source code for the `dtsr` Python module as well as support for reproducing published experiments.
Full documentation for the `dtsr` module is available at [http://dtsr.readthedocs.io/en/latest/](http://dtsr.readthedocs.io/en/latest/).

DTSR models can be trained and evaluated using provided utility executables.
Help strings for all available utilities can be viewed by running `python -m dtsr.bin.help`.
Full repository documentation, including an API, is provided at the link above.

Note that some published experiments below also involve fitting LME and GAM models, which require `rpy2` and therefore won't work on Windows systems without some serious hacking.
The `dtsr` module is cross-platform and therefore DTSR models should train regardless of operating system.

## Reproducing published results

This repository is under active development, and reproducibility of previously published results is not guaranteed from the master branch.
For this reason, repository states associated with previous results are saved in Git branches.
To reproduce those results, checkout the relevant branch and follow the instructions in the `README`.
Current reproduction branches are:

 - `emnlp18`
 - `naacl19`

Thus, to reproduce results from NAACL19, for example, run `git checkout naacl19` from the repository root, and follow instructions in the `README` file.
The reproduction branches are also useful sources of example configuration files to use as templates for setting up your own experiments, although you should consult the docs for full documentation of the structure of DTSR experiment configurations.

Published results depend on both (1) datasets and (2) models as defined in experiment-specific configuration files.
In general, we do not distribute data with this repository.
The datasets used can be provided by email upon request.

## Help and support

For questions, concerns, or data requests, contact Cory Shain ([shain.3@osu.edu](shain.3@osu.edu)).
Bug reports can be logged in the issue tracker on [Github](https://github.com/coryshain/dtsr).


## References
Shain, Cory and Schuler, William (2018). Deconvolutional time series regression: A technique for modeling temporally diffuse effects. _EMNLP18_.
