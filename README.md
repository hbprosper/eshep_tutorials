# Introduction
The jupyter notebook tutorials in this package complement the statistics/machine learning lectures given at the European School of High-Energy Physics. The tutorials provide a reasonably gentle, yet I hope highly instructive, introduction to a few important ideas in frequentist and Bayesian statistics as well as machine learning. Both fields are vast and increasingly complex. However, both contain ideas that are foundational and, therefore, remain valid. 

The tutorials implement solutions in Python to some of the more involved exercises presented in the lectures. 

The tutorials depend on a few well-known Python packages: 
  * __numpy__   (numerical analysis and array manipulation)
  * __pandas__  (data table manipulation)
  * __scipy__   (scientific comouting)
  * __matplotlib__ (plotting)
as well as on __ROOT__ (version 6.12.x), which includes the probability modeling package __RooFit__ and the statistical analysis package __RooStats__, which is built on top of __RooFit__.
  
In addition, the machine learning tutorials make use of  
  * __scikit-learn__ (an easy to use machine learning toolkit)
  
  
## Installation
I recommend that you create a directory called __external__ in your home directory with a standard linux code repository structure:
```
cd
mkdir -p external/bin
mkdir -p external/lib
mkdir -p external/include
mkdir -p external/share
```
You should clone all external packages, such as this one, in your __external__ directory. For the tutorials, you will need to execute the commands
```
cd
cd external
git clone https://github.com/hbprosper/eshep_tutorials
git clone https://github.com/hbprosper/eshep_tutorials
git clone https://github.com/hbprosper/dnnet
```
