# Linux (Ubuntu 14.04) Installation for CoLaboratory
Andee Kaplan & Eric Hare  
10/15/2014  

1. Install `python version 2.7`.
  - To check what version you have in terminal 
  
    ```
    python --version
    ```
  - To install, if it's not already
  
    ```
    sudo apt-get install python
    ```
2. Install `pip`
  - To install,
 
    ```
    sudo apt-get install python-pip
    ```
3. Install `python-dev`, `libzmq` and `libcurl`
  - To install,
  
    ```
    sudo apt-get install python-dev libzmq3-dev libcurl4-openssl-dev
    ```
4. Install `ipython notebooks`
  - To install,
  
    ```
    sudo pip install "ipython[notebook]"
    ```
    
5. Install `IRKernel`
  - To install, in R
  
    
    ```r
    #if not already installed
    install.packages("devtools")
    
    library(devtools)
    install_github('armstrtw/rzmq#8')
    install_github("takluyver/IRdisplay")
    install_github("takluyver/IRkernel")
    ```
6. Install CoLaboratory    
  - Clone CoLaboratory repo
 
    ```
    git clone --recursive git@github.com:jupyter/colaboratory.git
    ```
  - Run
    
    ```
    cd colaboratory
    pip install -r requirements.txt
    ```
7. Create R Profile
  - Clone this talk's repo (after getting out of the colaboratory directory)
    
    ```
    cd ..
    git clone git@github.com:andeek/presentations.git
    ```
  - Copy resources/profile_R to ~/.ipython/profile_R/
    
    ```
    mkdir ~/.ipython
    cp -rf presentations/isu-graphics/data_with_friends/resources/profile_R ~/.ipython/profile_R
    ```
