# Setting up Environments and Installing Packages Using Conda

## Summary of steps to complete

- [ ] Fork this repository so you have your own copy to work on.
- [ ] Clone the repository on your local machine. 
- [ ] Edit this README.md file on your machine.
- [ ] Run the Conda commands shown in the video and describe them in the table below.
- [ ] Push your changes to your GitHub repository.
- [ ] Submit a link to this GitHub repository in Canvas.

## 1. Fork & Clone this repository

* We did this in a previous assignment. Instructions are here: https://github.com/cmcntsh/exerGitPractice
* This can also be done directly in VSCode
  * Create a new folder on your machine where you want to put this repository if you don't already have one you want to use.
  * Copy the Clone or Download path for this repository from GitHub.
  * In VSCode from the command pallette (Ctrl-Shift-P) run Git: Clone
  * Paste the path into the path field which pops up
  * Select your new folder you created on your machine
  * A new folder for the repository with the repository files should be in the folder you selected showing in the Explorer window in VSCode on the left side.
  
## Edit your README.md file

* [ ] In an editor of your choice (i.e. VSCode) edit this README.md file to add the answers requested in the tables.

## Follow along with this tutorial

* Conda What and Why? (27 min): https://www.youtube.com/watch?v=23aQdrS58e0&list=PLG9A6ovzPqX6d9uWzx0UYN9pm0zzl5ofA&index=13&t=0s
  * He installs Miniconda. We will be using Anaconda. Don't install Miniconda.
  * Follow along with the rest of the tutorial.
  * Go ahead and create the environments as he creates them in the tutorial.

## Conda Concepts

* [ ] Describe the Conda concepts used in the video and listed in the table below.

|   Concept   |         Description or short answer         |
|     ---     |                     ---                     |
|What is the purpose of having different environments?     |environments are used to keep different programing purposes in python separate, like web design or data analysis|
|What is the default package manager in Python?            |pip - python  integrated package manager|
|How do you manage environments and packages in Anaconda?  |with the use of Conda which does both, but you can also use Conda for data analysis|
|`conda list`       |this shows all the default packages installed|
|`conda env list`       |this shows all the environments you have created|
|How do you keep your base environment unchanged?       |create different environments|
|What is the link to the Conda cheat sheet? (link in video notes is broken)      |https://conda.io/projects/conda/en/latest/user-guide/cheatsheet.html|
|`conda create --name XXXX`       |create and namea a new environment|
|`source activate XXXX`       |this activates the enviornment you want to use, must have the environment name, mine is "conda activate"|
|`conda install YYYY`       |this installs the packages you want to use, have to know the name of the package|
|channels in Conda       |the path or location where conda looks for packages|
|`conda install -c ZZZZ YYYY`       |install different channels were conda can look for packages|
|`conda config --show channels`       |this shows the channels installed which is the path that conda uses to look for packages|
|`conda config --add channels ZZZZ`       |this adds the channel to the channel list|
|conda-forge.org       |community led collection of packages only available from the forge website|
|`source deactivate`       |turns off whatever environment you are in and brings you back to your base environment|
|`conda config --get channels`       |this shows which channel will be searched frist, as they are given priotiues |

* After creating the environments he created in the video on your computer, what would the results of running the command `conda env list` look like with the da35 environment activated. Paste the output from your command prompt in the code block below.

```
(base) C:\Users\danni>conda activate da35

(da35) C:\Users\danni>conda env list
# conda environments:
#
base                     C:\Users\danni\anaconda3
ai378                    C:\Users\danni\anaconda3\envs\ai378
da35                  *  C:\Users\danni\anaconda3\envs\da35


```
* What command would you use to remove the environments you created for this exercise from your computer?

```
conda remove --name ai378 --all
conda remove --name da35 --all


```
