OLAFOAM
======

# Description

OLAFOAM is a new numerical model from the creator and developer of IHFOAM. This free and open source project is committed to bringing the latest advances in the simulation of wave dynamics to the OpenFOAM and FOAM-extend communities.

OLAFOAM is a set of solvers and boundary conditions to generate and absorb water waves actively at the boundaries and to simulate their interaction with porous coastal structures.

You can find all the information regarding the model at its web site and wiki:

https://sites.google.com/site/olafoamcfd/

https://openfoamwiki.net/index.php/Contrib/OLAFOAM

# Download and compilation

## Basic download guide

To get a full copy of OLAFOAM source and reference materials run in a terminal:

`git clone git://github.com/phicau/OLAFOAM.git`

Code updates can be downloaded in the future from the OLAFOAM folder as follows:

`git checkout`

`git pull`

## Basic compilation guide

First compile the boundary conditions:

`cd genAbs`

`./allMake`


Second compile the dynamic boundary conditions (currently it does not support all the versions):

`cd genAbs/waveGeneration/multiPistonMovement`

`./localMake`


Third compile the solvers (olaFoam and olaDyMFoam), selecting the correct folder for your preferred OpenFOAM/FOAM-extend version:

`cd solvers/olaFoamXXXXX`

`./allMake`

# Reference materials and tutorials

Reference materials and test cases are included in the OLAFOAM download. Check the *reference.zip* file and the *tutorials* folder. For a full description on these materials see:

https://openfoamwiki.net/index.php/Contrib/OLAFOAM#OLAFOAM_Documentation_and_Tutorials
