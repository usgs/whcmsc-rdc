# RDC
## RDC - Repository with Python Jupyter Notebooks for reductive dechlorination calculations

Christopher R. Sherwood, US Geological Survey

csherwood@usgs.gov

*See disclaimer and license in this repository.*

The calculations in these Python Jupyter notebooks investigate solutions to a multi-step reaction model describing the successive dechlorination of DDE to DDMU and finally to DDNU, as discussed in Eganhouse and Pontolillo (2008) and Eganhouse et al. (in review). The calculations produce Figures 7 and S-9 in the draft manuscript.

Eganhouse, R.P., J. Pontolillo (2008) Assessment of 1-chloro-4-[2,2-dichloro-1-(4-chlorophenyl)ethenyl]benzene (DDE) transformation rates on the Palos Verdes Shelf, CA,  *U.S.G.S. Open-File Report 2007-1362*, U.S. Geological Survey, Reston, VA, pp. 124.

Eganhouse, R.P., C.R. Sherwood, J. Pontolillo, B.D. Edwards, and P.J. Dickhudt (in review) Reductive dechlorination rates of 4,4’-DDE (1-chloro-4-[2,2-dichloro-1-(4-chlorophenyl)ethenyl]benzene) in sediments of the Palos Verdes Shelf, CA. Manuscript in review for submission to *Marine Chemistry*.

## Dependencies

The code uses several packages, including scipy, matplotlib, and numpy, which are standard in most Python distributions. It also requires lmfit (https://lmfit.github.io/lmfit-py/) which "provides a high-level interface to non-linear optimization and curve fitting problems".

Written in Python 3.6 in a Jupyter notebook. Run in a conda environment (https://conda.io/docs/intro.html) created with the `environment.yml` file included in the repository using the command `conda env create -f environment.yml`. Specific documentation of the Python environment used is contained in the file `specific_environment.txt`, generated with the command `conda list --explicit > specific_environment.txt`.


## Batemen
The name of the notebooks refers to Harry Bateman, FRS, who provided analytical solutions for multi-step radioctive decay. The analytical solutions were not used here because they are indeterminiate when two of the rate constants are identical, which can happen in the course of the minimization procedure.

https://en.wikipedia.org/wiki/Bateman_Equation


Bateman, H. (1910) The solution of a system of differential equations occurring in the theory of radio-active transformations, *Proc. Cambridge Phil. Soc.* 15(V):423-427.

Keegan, R.P. and R.J. Gehrke (2003) A method to determine the time since last purification of weapons grade plutonium *Applied Radiation and Isotopes* 59:137-143.

