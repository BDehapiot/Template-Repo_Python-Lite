![Python Badge](https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=rgb(149%2C157%2C165)&labelColor=rgb(50%2C60%2C65))  
![Author Badge](https://img.shields.io/badge/Author-Benoit_Dehapiot-blue?labelColor=rgb(50%2C60%2C65)&color=rgb(149%2C157%2C165))  
![License Badge](https://img.shields.io/badge/Licence-GNU_General_Public_License_v3.0-blue?labelColor=rgb(50%2C60%2C65)&color=rgb(149%2C157%2C165))  


# Template-Repo_Python-Lite
## Description

## Installation
This tutorial provides a step-by-step guide to install **Python**, coupled with **Spyder**, using the **Mamba/Conda** environment manager.  

Spyder is an Integrated Development Environment (IDE), allowing users to easely execute and interact with Python codes. Although not mandatory, Spyder is recommended for beginners.  

Please select your operating system:

<details> <summary>Windows</summary>  

<br>While all the following steps are required for installation, only steps 5, 8 and 9 will be required subsequently. 

### Download GitHub repository:  

1) Download GitHub repository
([link](https://github.com/BDehapiot/ETH-ScopeM_CZITools/archive/refs/heads/main.zip)) 

2) Unzip folder to a known location (e.g. `C:\Users\YourUsername\Desktop`)

### Install Mambaforge:  

3) Download Mambaforge installer for Windows
([link](https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Windows-x86_64.exe))  

4) Run the downloaded `.exe` file and select the following options:    
    - create start menu shortcuts  
    - add Miniforge3 to PATH environment variable  

### Setup Mamba/Conda environment: 

5) Run `Miniforge Prompt` from start menu shortcuts (see `Miniforge3` folder)  
<br>The prompt should look like this:  
    ```bash
    (base) C:\Users\YourUsername>
    ```
    `(base)` at the beginning of the prompt means that you are in your base environment

6) Move to the downloaded GitHub repository using the `cd` command: 
    ```bash
    cd Desktop/Template-Repo_Python-Lite-main
    ```
    The prompt should change to reflect your current location:
    ```bash
    (base) C:\Users\YourUsername\Desktop\Template-Repo_Python-Lite-main>
    ```

7) Create a new Mamba/Conda environment (takes a few minutes): 
    ```bash
    mamba env create -f environment.yml
    ```

8) Activate the newly created environment:
    ```bash
    mamba activate Python-Lite
    ```

    The prompt should now start with `(Python-Lite)`
    ```bash
    (Python-Lite) C:\Users\YourUsername\Desktop\Template-Repo_Python-Lite-main>
    ```

### Start and setup Spyder IDE: 

9) Start Spyder using the following command:
    ```bash
    spyder
    ```

10) Create a new Spyder project
    - Click the `Projects` > `New Project...`
    - Choose `Existing directory`
    - Select the GitHub repository using the folder icon
    - Click the `Create` button  

    You can re-open your project later using `Projects` > `Recent Projects...`
</details>  

<details> <summary>MacOS</summary>  

<br>While all the following steps are required for installation, only steps 4, 10 and 11 will be required subsequently. 

### Download GitHub repository:  

1) Download GitHub repository
([link](https://github.com/BDehapiot/ETH-ScopeM_CZITools/archive/refs/heads/main.zip)) 

2) Unzip folder to a known location (e.g. `~/Desktop`)

### Install Mambaforge:  

3) Download Mambaforge installer for MacOS 
([legacy](https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-MacOSX-x86_64.sh))
([M-Series](https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-MacOSX-arm64.sh))    

4) Open your terminal (typing 'terminal' in `Launchpad` or `Spotlight search`)  
<br>The prompt should look like this:
    ```bash
    YourUsername@MacBook-Pro ~ %
    ```

5) Move to the directory where the downloaded Miniconda script is located (most likely your `Downloads` folder)
    ```bash
    cd ~/Downloads
    ```
6) Run the script using the following `bash` command followed by the name of the file `.sh` you downloaded:  
    Legacy
    ```bash
    bash Miniforge3-MacOSX-x86_64.sh
    ```
    M-Series
    ```bash
    bash Miniforge3-MacOSX-arm64.sh
    ```
    Follow the Terminal prompts to complete the installation and accept default options  

### Setup Mamba/Conda environment: 

7) Close and re-open your terminal  
    <br>The prompt should now look like this:
    ```bash
    (base) YourUsername@MacBook-Pro ~ %
    ```
    `(base)` at the beginning of the prompt means that you are in your base environment

8) Move to the downloaded GitHub repository using the `cd` command: 
    ```bash
    cd Desktop/Template-Repo_Python-Lite-main
    ```
    The prompt should change to reflect your current location:
    ```bash
    (base) YourUsername@MacBook-Pro Desktop/Template-Repo_Python-Lite-main %
    ```

9) Create a new Mamba/Conda environment (takes a few minutes):  
    ```bash
    mamba env create -f environment.yml
    ```

10) Activate the newly created environment:
    ```bash
    mamba activate Python-Lite
    ```

    The prompt should now start with `(Python-Lite)`
    ```bash
    (Python-Lite) YourUsername@MacBook-Pro Desktop/Template-Repo_Python-Lite-main %
    ```

### Start and setup Spyder IDE: 

11) Start Spyder using the following command:
    ```bash
    spyder
    ```

12) Create a new Spyder project
    - Click the `Projects` > `New Project...`
    - Choose `Existing directory`
    - Select the GitHub repository using the folder icon
    - Click the `Create` button  

    You can re-open your project later using `Projects` > `Recent Projects...`
</details>  

## Dependencies
### Conda
- python=3.10
- numpy
- scipy
- scikit-image
- pandas
- opencv
- joblib
- matplotlib-base
- pyyaml
- pip

### pip
- napari[all]
- spyder
