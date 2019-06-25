# TMVA Tutorial

THESE TUTORIALS ARE NOT THE PROPERTY OF PRIVDONUT123, BUT MERELY COPIED FOR SELF REFERENCE

These are tutorials on TMVA given at the IML workshop (20-22 March 2017)

See  https://indico.cern.ch/event/595059


The tutorials consist of notebook which can be run on SWAN ( https://swan.cern.ch )


In order to run the tutorial we recommend that you:

1. Open a Terminal in SWAN 
2. Clone your repository (it will appear in your cernbox folder)
```
git clone https://github.com/lmoneta/tmva-tutorial.git
```

* The notebooks used in this tutorial use the Python interface of ROOT (PyROOT) and the Javascript based extension for notebook, `JSMVA`.

* More notebooks, some written also in C++, are available in the Machine Learning Gallery of SWAN, https://swan.web.cern.ch/content/machine-learning

* Addition tutorials of TMVA are available in the `tutorials/tmva` directory of the main ROOT git repository. These are available also here https://root.cern.ch/doc/master/group__tutorial__tmva.html

* The updated TMVA Users Guide is available on git, https://github.com/root-project/root/raw/master/documentation/tmva/UsersGuide/TMVAUsersGuide.pdf

## Swan and Jupyter notebooks quick start ##

If you never used jupyter notebooks, you can find some quickstart information at the following links [What is a jupyter notebook?](http://nbviewer.jupyter.org/github/jupyter/notebook/blob/master/docs/source/examples/Notebook/What%20is%20the%20Jupyter%20Notebook.ipynb), [Notebook Basics](http://nbviewer.jupyter.org/github/jupyter/notebook/blob/master/docs/source/examples/Notebook/Notebook%20Basics.ipynb),  [Running Code](http://nbviewer.jupyter.org/github/jupyter/notebook/blob/master/docs/source/examples/Notebook/Running%20Code.ipynb).

For information on swan, see the swan website: https://swan.web.cern.ch
In a nutshell, "SWAN (Service for Web based ANalysis) is a platform to perform interactive data analysis in the cloud". It gives you access to the LCG software stacks and to your CERNBOX files. 

* You need to have an active **CERNBOX** to use swan (https://cernbox.cern.ch/). If you don't have a CERN account, please contact us directly and some temporary accounts can be made available. 

* If you think think the Jupyter notebook is stuck, open a terminal on swan and execute `top`: if the cpu is not being used (0%) by any of your processes, you may have to restart the Jupyter
kernel.

* There is a known issue when executing `import ROOT` in a Python notebook, which may get stuck.  However this problem should not be present anymore with the latest development version of SWAN.


**IMPORTANT:**    
* Please only have one notebook at the time on swan (you have to select the "running" tab and shutdown the notebook when done)
* Please avoid Chrome, it has known problems restarting kernels.
* Limit the number of events you use on swan (order 10000-100000) and the avoid expensive methods: *swan is meant for fast prototyping*. 
     * Each swan container has 2 GB of ram assigned, using the full dataset may hit the memory limit.

