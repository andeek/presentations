# Mac OSX Installation for CoLaboratory
Andee Kaplan & Eric Hare  
10/15/2014  

1. Install `python version 2.7` (should already be installed, if so skip to 2.)
  - To check what version you have in terminal 
  
    ```
    python --version
    ```
  - To install, if it's not already
  
    ```
    https://www.python.org/download/
    ```
2. Install `homebrew`
   - To install,
 
    ```
    ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    ``` 
3. Install `pip`
  - To install,
 
    ```
    sudo easy_install pip
    ```
4. Install `ipython notebooks`
  - To install,
  
    ```
    sudo pip install "ipython[notebook]"
    ```
5. Install `libzmq` with `homebrew`
  - To install or upgrade,
  
    ```
    brew install zmq
    
    # or upgrade
    brew update
    brew upgrade zmq
    ```
    
6. Install `IRKernel`
  - To install, in R
  
    
    ```r
    #if not already installed
    install.packages("devtools")
    
    library(devtools)
    install_github('armstrtw/rzmq#8')
    install_github("takluyver/IRdisplay")
    install_github("takluyver/IRkernel")
    ```
7. Install CoLaboratory    
  - Clone CoLaboratory repo
 
    ```
    git clone --recursive git@github.com:jupyter/colaboratory.git
    ```
  - Run
    
    ```
    cd colaboratory
    pip install -r requirements.txt
    ```
8. Create R Profile
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
