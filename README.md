<!--

When you have set up your repo

**Unit tests and coverage**

[![](https://img.shields.io/badge/Octave-CI-blue?logo=Octave&logoColor=white)](https://github.com/Remi-gau/template_matlab_analysis/actions)
![](https://github.com/Remi-gau/template_matlab_analysis/workflows/CI/badge.svg)

[![codecov](https://codecov.io/gh/Remi-gau/template_matlab_analysis/branch/master/graph/badge.svg)](https://codecov.io/gh/Remi-gau/template_matlab_analysis)

**Miss_hit linter**

[![Build Status](https://travis-ci.com/Remi-gau/template_matlab_analysis.svg?branch=master)](https://travis-ci.com/Remi-gau/template_matlab_analysis)

-->

# CPP source MRI

This is a set of functions to prepare a source fMRI dataset for BIDSification and analyses

This can perform:

- 3D to 4D nii files conversion

- anatomical defacing [ W I P ]

- gzip the nii files in a BIDS raw folder

The core functions are in the `src` folder. This set of functions is intended to be added manually
as a submodule to the analysis repo forked from
[template_fMRI_analysis](https://github.com/cpp-lln-lab/template_fMRI_analysis)

## How to install and use this template

### Add as a submodule

1. Open the terminal and navigate to your analysis folder forked from
[template_fMRI_analysis](https://github.com/cpp-lln-lab/template_fMRI_analysis) and cloned locally

2. Type

```bash
# navigate to the `lib` folder
cd lib

# add the submodule
git submodule add https://github.com/cpp-lln-lab/CPP_sourceMRI

# initialize the nested submodule(s)
git submodule update --init --recursive
```

3. commit the new changes (the new submodule(s))

### Dependencies

Make sure that the following toolboxes are installed and added to the matlab
path.

For instructions see the following links:

<!-- lint disable -->

| Dependencies                                                                              | Used version |
| ----------------------------------------------------------------------------------------- | ------------ |
| [Matlab](https://www.mathworks.com/products/matlab.html)                                  | 20???        |
| or [octave](https://www.gnu.org/software/octave/)                                         | 4.?          |
| [SPM12](https://www.fil.ion.ucl.ac.uk/spm/software/spm12/)                                | v7487        |
| [CPP_SPM](https://github.com/sergivalverde/nifti_tools)*                                  | > 0.1.0      |

\*already "installed" in [template_fMRI_analysis](https://github.com/cpp-lln-lab/template_fMRI_analysis) and cloned locally

<!-- lint enable -->

## Contributing

Feel free to open issues to report a bug and ask for improvements.

If you want to contribute, have a look at our
[contributing guidelines](https://github.com/cpp-lln-lab/.github/blob/main/CONTRIBUTING.md)
that are meant to guide you and help you get started. If something is not clear
or you get stuck: it is more likely we did not do good enough a job at
explaining things. So do not hesitate to open an issue, just to ask for
clarification.
