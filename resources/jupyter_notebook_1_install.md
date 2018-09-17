# Jupyter Notebook:  Getting Started
The Jupyter notebook is an interactive computational environment, in which you can combine code, execution, rich text, mathematics, plots and rich media. 

---

### [Install the Notebook](http://jupyter.readthedocs.io/en/latest/install.html)
Installing Jupyter using Anaconda and conda:  
For new users, we highly recommend [installing Anaconda](https://www.continuum.io/downloads). Anaconda conveniently installs Python, the Jupyter Notebook, and other commonly used packages for scientific computing and data science.  (Prereq: Python is installed.)

Once anaconda is installed, you can launch the notebook by typing
```{bash}
$ jupyter notebook
```

### Upgrade all libraries/packages
We will now update all the packages/libraries installed by anaconda to ensure you have the latest version of everything!

```{bash}
$ conda update --all
```

### Run the Notebook at Terminal Prompt  
Note:  The notebook will open at the directory in which you launch the notebook on your terminal.  
```
$ jupyter notebook
```
>```
>users-MBP:pandas user$ jupyter notebook
>[I 15:30:20.559 NotebookApp] JupyterLab extension loaded from /Users/user/anaconda3/lib/python3.6/site-packages/jupyterlab
>[I 15:30:20.559 NotebookApp] JupyterLab application directory is /Users/user/anaconda3/share/jupyter/lab
>[I 15:30:20.566 NotebookApp] Serving notebooks from local directory: /Users/user/Documents/Data_Science/Github/dsp/python/pandas
>[I 15:30:20.566 NotebookApp] The Jupyter Notebook is running at:
>[I 15:30:20.566 NotebookApp] http://localhost:8888/?token=ddeb5deeac4357ca04a11200b89116360d1c75ab78d730e3
>[I 15:30:20.566 NotebookApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
>[C 15:30:20.567 NotebookApp] 
>```
```console
reshama$ jupyter notebook
[I 11:41:22.769 NotebookApp] Serving notebooks from local directory: /Users/reshamashaikh/_ds/metis
[I 11:41:22.769 NotebookApp] 0 active kernels 
[I 11:41:22.769 NotebookApp] The Jupyter Notebook is running at: http://localhost:8888/
[I 11:41:22.769 NotebookApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
```

### Shut Down the Juypter Notebook App
At terminal prompt:  
 * control + c
 * type:  `y`

>```console
>^C[I 15:33:01.661 NotebookApp] interrupted
>Serving notebooks from local directory: /Users/user/Documents/Data_Science/Github/dsp/python/pandas
>0 active kernels
>The Jupyter Notebook is running at:
>http://localhost:8888/?token=ddeb5deeac4357ca04a11200b89116360d1c75ab78d730e3
>Shutdown this notebook server (y/[n])? y
>[C 15:33:05.559 NotebookApp] Shutdown confirmed
>[I 15:33:05.560 NotebookApp] Shutting down 0 kernels
>users-MBP:pandas user$ 
>```
```console
^C[I 11:43:35.486 NotebookApp] interrupted
Serving notebooks from local directory: /Users/reshamashaikh/_ds/metis
0 active kernels 
The Jupyter Notebook is running at: http://localhost:8888/
Shutdown this notebook server (y/[n])? y
[C 11:43:37.782 NotebookApp] Shutdown confirmed
[I 11:43:37.783 NotebookApp] Shutting down kernels
reshama$ 
```

---

### Getting to Know Jupyter

You can try out Jupyter on a browser without installing it.  
https://try.jupyter.org/

