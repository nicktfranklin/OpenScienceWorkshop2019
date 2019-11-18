# OpenScienceWorkshop2019
Welcome to the Open Science Workshop Github Repository!

This repository contains some simple examples of how code, specifically, *Jupyter Notebooks*, integrate with Github and and be run online. 


This repository has two demonstrations for hosting code online (see below).  

## Structure of a Respository
___
In general, there are several key files you will tend to see over and over in GitHub Repositories:
  
  * README.MD file
  * requirements.txt
  * LICENSE
  * .gitignore

The `README.MD` file is a description of your repository (more on that below). 

The `requirements.txt` file is typically a list of python packages that the repository can use.  These are typically compatable with the pip package mananger ([documentation here](https://pip.readthedocs.io/en/1.1/requirements.html)), but the important point is to make sure that somewhere in the repository, it is clear exactly what is needed to run your code.  The specifics of that are less important.  

The `LICENSE` file is common, but generally not necessary for smaller projects.  I've chosen the MIT license, and GitHub makes it easy to choose among several.  There is more information [here](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/licensing-a-repository), but generally this is something you don't need to worry too much about unless you are building software.

The `.gitignore`  file list all of the files that you don't want to include in the reposistory. A lot of programs create temporary and/or hidden files (often starting with a '.') that can clutter a repository.  The `.gitignore` specifies files to ignore for the purposes of version control. 

### What can you host in GitHub?
(Almost) anything! GitHub suggests that repositories are less than 1GB and limits all files to a maximum of 100 MB.  It's a great place for non-sensitive data, analyses, simulations, presentations, websites, etc.  

Use your Github for whatever you want.  It is an easy way to share files, with special tools for code, and specifically, python code.

## Documenting your Github
___
What you are reading now is the 
`README.MD` file.  This file is written in *Markdown*, a simplified HTML-based langauge that allows you to quickly and easily write a website. With markdown, you can quickly add links, basic formatting, even code and laTex script. Github will automatically render any file named README.MD in the body of the respository. You can see the raw markdown for this README.MD file: [raw markdown](https://raw.githubusercontent.com/nicktfranklin/OpenScienceWorkshop2019/master/README.md).


Here is what mathematical notation looks like rendered:

$$x \sim N(\mu, \sigma)$$

and code:

```
def my_fun(a, b):
    return a + b
```


and here's a fun photo of me and a llama:

<img src="images/IMG_0488.png" alt="Kitten"
	title="Nick and a Llama" width="150" height="150" />
<!-- Here, I use a standard HTML tag to imbed the image so I could resize it. You can also use the following code to imbed images, but with less control:


![image nick_llama](/images/IMG_0488.png)

 -->


The point is you can do a lot with Markdown very easily.  Your `README.MD` file can be as expressive as you like, and having a well documented and detailed `README.MD` file can really help make your work intelligable to someone else.


Here is a good guide on writting Markdown in README.MD files: [Mastering Markdown](https://guides.github.com/features/mastering-markdown/).  Markdown 

## Hosting code online
___
You have a couple of options that allow you to host the code in your repository online so that others can use the code without going through a time-consuming installation process.  Making sure that your code will run on someone else's computer can be a huge pain point, but luckily, there are two good and easy solutions for hosting python code within Jupyter notebooks: [Binder](https://mybinder.org) and [Google Colab](https://colab.research.google.com/)

### Binder

[Binder](https://mybinder.org) is a resource for running Jupyter notebooks online. It integrates directly with github and will install any packages listed in your `requirements.txt`.  It creates a Docker image of your repository and allows you to run your code online.


We've created an example notebook to use with [Binder](https://mybinder.org).  This example looks at the problem of change-points and how a simple reinforcement learning model handels them:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nicktfranklin/OpenScienceWorkshop2019/master?filepath=JupyterNotebooks%2FChangePointDetection%20Demo.ipynb) 


### Google Colab


[Google Colab](https://colab.research.google.com/) is simliar, but more powerful.  Colab has many packages pre-installed and comes with access to GPUs, making it ideal for sharing neural networks.  


Below, we have a tutorial on writting code that's user-friendly and with some helpful functions in Colab.

<a href="https://colab.research.google.com/github/nicktfranklin/OpenScienceWorkshop2019/blob/master/JupyterNotebooks/SimpleColab_OpenScienceWorkshop.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab" title="Open and Execute in Google Colaboratory"></a> 

#### Deep Learning in Colab
One of the nice things about Colab is that you can use GPUs for free to run distributed computing software like Tensorflow and PyTorch.  Google has a number of excelent tutorials for this in the main page ([here](https://colab.research.google.com/)), but here is demonstration a Variational Autoencoder processing handwritten digits: [link](https://colab.research.google.com/github/tensorflow/docs/blob/master/site/en/tutorials/generative/cvae.ipynb)
