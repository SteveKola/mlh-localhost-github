## Circumventing the Errors of Installing Jupyter Notebook on Older and Smaller Computers.

**A guide on that explains how to install Jupyter Notebook, even when your PC is optimal.
**

How many people have you encountered, that gave up on coding because they lack the hardware resources or faced installation issues?

In recent times, I've come across a large number of individuals who are passionate to learn, but are almost always hindered by limited resources. I've anchored a number of Python and ML classes these days, and I realized that the easiest and commonest block for coding beginners is installation issues.

I'd been able to help figure a way out for about 98% of the people that had approach me to help with installation problems. But there are lots more people who I haven't been opportune to meet physically, hence, the reason for this guide.

In this guide, I will expound on the different errors that can be encountered while installing Jupyter notebook, and how they can be solved. I will also explain how you can use Jupyter notebook on your smartphone, in case you don't have a PC or you wish for more coding time than your PC can offer.

## I'm a beginner and I don't know any programming terms. WTF is Jupyter Notebook?

Jupyter Notebook is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text.

![1.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1586553584365/OlMVdYtra.png)

Uses include: data cleaning and transformation, numerical simulation, statistical modeling, data visualization, machine learning, and much more.

## Different ways of Installing Jupyter Notebook.

Jupyter Notebook can either be installed through Anaconda or via PIP command.

Anaconda Distribution is the easiest way to perform Python/R data science and machine learning on PCs. (And highly recommended for beginners, too).

![2.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1586553618460/YA2XJP0b0.png)

It provides a large selection of packages (including Jupyter notebook) that are pertinent to your workflow as a Data Scientist.

Installing Jupyter Notebook via PIP command is a manual way of installing Jupyter notebook. You get not to install numerous libraries that you'd probably never need, but would come as part of the whole Anaconda package.

If you are a beginner, and you have a PC with a minimum of 2GB RAM, I'd recommend installing Anaconda.

If your PC is not so powerful, and/or you know your way around a terminal (command prompt, in Windows), you may want to use PIP for your Jupyter notebook installation.

Now that we understand all the big terminologies, we should dive into the errors, right?

## Different Errors You might Faced during Installation.

### i. Fail to Create Start Menu.

![3.jpeg](https://cdn.hashnode.com/res/hashnode/image/upload/v1586553642864/n6ht0Ln3q.jpeg)

This is the most prevalent error while installing Jupyter notebooks.
By my observations, this error usually occur when installing Anaconda on a PC running on Windows 7 OS. I have encountered this error on just one Windows 8 PC. But never on a PC on Windows 10 OS.

My postulation is that the newer versions of Anaconda don't work well with Windows 7. There are 2 solutions to this;

- Download an earlier version of Anaconda that supports Windows 7. Anaconda 2019.03 is the round peg. Click  [here](https://repo.anaconda.com/archive/) , navigate to where 2019.03 is, and download the suitable version for your PC.
- Second solution is to upgrade the PC's operating system to Windows 10 and try reinstalling Anaconda. It should work like a magic!

### ii. Jupyter notebook displaying a blank page when loaded.

![4.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1586553661454/8OPiGSpY5.png)

There is a very tiny possibility that you might encounter this error. The fix is to install an older version of Jupyter notebook. Copy and paste the command below.

```
pip install notebook==5.7.4
``` 

And you'd be fine.

### iii. My PC is too old or small to Install Anaconda.

Why then! I have your medicine! 

If for one reason or the other, your PC is too slow/small to run Anaconda. You can always install via PIP. PIP is an acronym for Pip Install Packages. *Sounds meta, if you'd ask me.*

For you to be able to use PIP, you need to install Python on your PC. Click  [here](https://www.python.org/downloads/)  to download Python and get it install on your PC. Make sure you add Python to PATH.

![5.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1586553695250/EYTDK2nc2.png)

While Trying to Install Python, you might come across this error;

![6.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1586553717529/xbMaRFRh0.png)

Update your Windows and try installing Python again.

To update your Windows, press the Windows button on your PC and type "Windows Update". Click on Windows Update. Click on Search for Updates.

By then it should bring up a list of updates to install. Install them and try reinstalling Python once the updates have been installed.

Once you are done installing Python, you can check if Python is installed on your PC by opening your command prompt and typing;

``` 
python --version
``` 

![7.jpeg](https://cdn.hashnode.com/res/hashnode/image/upload/v1586553759122/79dlDdrok.jpeg)

If *python --version* doesn't work, you may try;
```
py --version
``` 

If you have something like the one below, it means that Python is not installed on your PC. Go back up, follow the instructions carefully and try again.

![8.jpeg](https://cdn.hashnode.com/res/hashnode/image/upload/v1586553784247/VTO6n_5sq.jpeg)

**Note: ** Make sure that Python is installed before you go further.

Check if PIP is installed (which it should be) by typing;
```
pip --version
``` 

You should see a response prompt similar to that of  *py --version*.

If you see something like,
``` pip is not a recognized command
``` that translates to Python not being added to PATH.

Click  [here](https://datatofish.com/add-python-to-windows-path/)  to see how you can add Python and PIP on your computer path.

In case you don't want to bother, prefix all your PIP commands with 
```py -m
``` . For example typing 
```py -m pip --version
```  instead of 
```py -m 
``` to display your PIP version.

Once you are done, you can now install Jupyter notebook using;

```
pip install jupyter
``` 

If, for any reason apart from bad internet connectivity, Jupyter notebook is not installing, try out the following commands.

``` 
pip install setuptools
pip install python-language-server
```

**NOTE:** Remember to prefix the PIP commands with py -m if Python is not added to PATH.

Once you are done with these above commands, try pip install jupyter again.

Once you are done, you'd need to install the libraries that you'd be working with as a Data Scientist. Most of these libraries usually come along with the Anaconda distribution, but since we are installing manually…

We'd focus on just Numpy, Pandas, Scikit Learn, Matplotlib and Seaborn. If, as you progress in your journey as a Data Scientist, you find a new libraries that you'd want to work with, it can easily be installed using pip install.

Copy and paste the following commands;

```
pip install pandas
pip install sklearn
pip install seaborn
``` 

Installing Pandas will install Numpy automatically, as Pandas is built on Numpy. Likewise, installing Seaborn will install matplotlib automatically, as Seaborn is built on Matplotlib.

Once the libraries are all installed, you can now open your Jupyter notebook by typing 
``` 
jupyter notebook 
``` 
in your command prompt.

![9.jpeg](https://cdn.hashnode.com/res/hashnode/image/upload/v1586553826306/aR5oydaS5.jpeg)

And viola! It'd open jupyter notebook right in your default browser.

![10.jpeg](https://cdn.hashnode.com/res/hashnode/image/upload/v1586553845122/BeKXogUCG.jpeg)

**NOTE:** In case your PIP is not installed on PATH, you'd have to prefix every command with *py -m*. E.g.

```
py -m jupyter notebook
``` 

### iv. Other minute Errors

There might be cases where you have been using Anaconda for a while and you suddenly started facing errors like jupyter kernel not loading, …, etc.

The fastest fix is to uninstall Anaconda and then reinstall it. The method works every single time I've tried it on our students' PCs.

### v. The Fix that would work when Others Fail.

Install a Linux distro (distro for distribution).

If Anaconda is running too slowly on your PC, or for a strange reason, none of these fixes work on your PC. You can always replace your Windows OS with a Linux distro.

Windows are infamously known to hog the average PC's resources. Linux distros are usually lighter and faster than Windows on older machines.

In fact, you could run Jupyter notebook on a PC of even 512mb RAM, if it is running on one of the lighter-weight Linux distros.

Since you'd be coming from a Windows background, I'd recommend you porting to either  [Ubuntu MATE](https://ubuntu-mate.org/download/)  or  [Linux Mint](https://www.linuxmint.com/download.php) .

The two Linux distros possess Windows-like GUI and are breath of fresh air. I know because I've used both.

One other advantage is that Python usually come preinstalled in Linux. Quite a number of Linux functionalities are dependent on Python. All you have to do is to upgrade PIP and, easy!

This article is longer than I intended, so I'd write another article explaining how to install Jupyter notebook on your smartphone. You can read the article  [here](https://steventure.hashnode.dev/coding-made-easy-use-jupyter-notebooks-on-smartphones-ck8uox9ut0094l6s1g17dpz2k) .

## Finally…

Don't give up on your coding dreams because of something as niggling as installation issues. We don't give up, folks.

Do well to click on the several buttons here, if you find this article insightful. You may also connect with me on  [LinkedIn](https://www.linkedin.com/in/steven-kolawole-80/)  and  [Twitter](https://twitter.com/steveddev) .

Thank you for reading.