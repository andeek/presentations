Data analysis with friends (Part 1)
========================================================
author: Eric Hare & Andee Kaplan
date: October 15, 2014

<img src="images/data-with-friends.png" height=150/>

Real-time data analysis together
=========================================================

**What**: ISU Graphics group will host a 1 hour data-a-thon in which we will all analyze a dataset together.

**When**: Nov. 5th at 1:10pm

**Where**: In Snedecor 2113 (remote participants also encouraged to participate)

**Why**: For the fun of it.

Today we will discuss **how** this will be accomplished.

What is IPython?
========================================================
Rich architecture for interactive computing with:
- Powerful Python shells (terminal and Qt-based).
- A web-based notebook with the same core features but support for code, text, mathematical expressions, inline plots and other rich media.
- Support for interactive data visualization and use of GUI toolkits.
- Flexible, embeddable interpreters to load into your own projects.
- Easy to use, high performance tools for parallel computing.

[[Source]](http://ipython.org/)

IPython \(\rightarrow\) Project Jupyter
========================================================
<img src="images/jupyter-logo.png" height=70 />

Created in Summer 2014 by the IPython development team to carry forward a vision of reproducible interactive computing for all programming languages:
- Python
- Julia
- R
- Ruby, Haskell, Scala, Go, etc.

Jupyter goals
=========================================================
A home for the language independent parts of the architecture:
- A network protocol for applications to talk to kernels that run code for interactive computations.
- A set of applications that enable users to write and run code on those kernels.
- Notebook file format and conversion tools (nbconvert).
- Notebook sharing service (https://nbviewer.jupyter.org/).

[[Source]](http://nbviewer.ipython.org/github/ellisonbg/talk-2014-summer/blob/master/Jupyter%20and%20IPython.ipynb)

CoLaboratory
=======================================================
Create and store notebooks in Google Drive and allow for collaborative editing of notebooks using

1. The CoLaboratory Chrome App.
2. CoLaboratory with Classic Jupyter Kernels.

**Requirements**
- Chrome Beta or Dev version
- IPython version 2.x (Not 3.0!)

Choose your own adventure (kernel)!
=======================================================
- `IRKernel` is a package that allows us to run a CoLaboratory (Jupyter) notebook with an `R` kernel.
- **Your turn**: Let's get CoLaboratory up and running so we can all play!

Operating System | Installation Guide
-----------------|-------------------
Linux (Ubuntu 14.04) | <a href="resources/linux_installation.html" target="_blank">click</a>
Mac OSX | <a href="resources/macosx_installation.html" target="_blank">click</a>
Windows 7/8 | Find a friend.

After successful installation
=======================================================
1.  

  ```
  cd /path/to/colaboratory
  python -m colaboratory --profile R
  ```
2. Log in with your google drive account
3. E-mail your google drive account name to `andee.kaplan@gmail.com`
4. Open the document we share with you
...

5. Data party!!
=======================================================
![Nerd Party](images/partyhard.gif)
