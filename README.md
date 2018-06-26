# Introduction
The jupyter notebook tutorials in this package complement the statistics/machine learning lectures given at the __European School of High-Energy Physics__. The tutorials provide a reasonably gentle, yet I hope highly instructive, introduction to a few important ideas in frequentist and Bayesian statistics as well as machine learning. Both fields are vast and increasingly complex. However, both contain ideas that are foundational and, therefore, remain valid. 

The tutorials implement solutions in Python to some of the more involved exercises presented in the lectures. 

The tutorials depend on a few well-known Python packages: 
| modules       | comment     |
| :---          | :---        |
| pandas        | data table manipulation, often with data loaded from csv files |
| numpy         | array manipulation and numerical analysis      |
| scipy         | scientific computing    |
| matplotlib    | a widely used plotting module for producing high quality plots |
| pylab         | embedded within matplotlib and provides Matlab-like features |
| scijit-learn  | easy to use machine learning toolkit |

The tutorials also use __ROOT__ (version 6.12.x), which includes the probability modeling package __RooFit__ and the statistical analysis package __RooStats__, which is built on top of __RooFit__.
 
  
  
## Installation
I recommend that you create a directory called __external__ in your home directory with a standard linux code repository structure:
```
cd
mkdir -p external/bin
mkdir -p external/lib
mkdir -p external/include
mkdir -p external/share
```
You should clone all external (utility) packages into your __external__ directory. For the tutorials, you will need to execute the commands
```
cd
mkdir -p Projects/Tutorials
cd Projects/Tutorials
git clone https://github.com/hbprosper/eshep_tutorials

cd
cd external
git clone https://github.com/hbprosper/histutil
git clone https://github.com/hbprosper/dnnet
```
The first package is this one, containing the tutorials. Do not place this in __external__. Put it in some work area, e.g., __$HOME/Projects/Tutorials__. The second package is a collection of simple utilities that use __ROOT__, while the third can be used to create a C++ file that encapsulates a fully connected feed forward deep neural network fitted (trained) using __scikit-learn__'s __MLPClassifier__ class. Once per terminal session, you should do
```
source $HOME/external/histutil/setup.sh
source $HOME/external/dnnet/setup.sh
```
This works for a __bash__ shell. If you use another shell, I'm afraid you'll have to create your own versions of the setup.sh scripts. Sorry! Ok, you're ready to rumble!

# Tutorials
There are two directories in this package, __stats__ and __ml__. The first contains the notebooks
```
00.1_roofit.ipynb
00.2_roofit.ipynb
07.1_rootn.ipynb
07.2_poisson.ipynb
08_bias.ipynb
09_wilks.ipynb
11_16_hzz4l.ipynb
```
and second contains the notebooks
```
00_prepare_hzz_data.ipynb
01_bdt_wine.ipynb
01_dnn_wine.ipynb
02_dnn_hzz_vbf_ggf.ipynb
03_hmc.ipynb
```

