# BAESCM

BAESCM was proposed for estimating land cover areas in subregions, through downscaling the global sample information to subregion scale. Moreover, a semi-empirical method for inferring the confidence intervals of the estimated areas was introduced.  
  
For the flexibility and scalability, the code was implemented with Google Earth Engine of Python format, not JavaScript format.    

If you have not used Google Earth Engine of Python format before, please follow the steps in "Environment configuration" section to install and configure the packages; if you have used it before, you can directly skip to the "Run the code" section.    
## Environment configuration

1. Install Miniconda/[Anaconda](https://www.anaconda.com/download)
2. Create and activate a Conda environment：
   ```bash
   conda create -n gee python=3.10
   conda activate gee
   ```
3. Geemap installation：  
   3.1 install mamba:
   ```bash
   set PYTHONUTF8=1
   conda install -c conda-forge mamba
   ```
   3.2 install geemap:
   ```bash
   mamba install -c conda-forge geemap pygis
   ```
4. Geemap configuration:  
   4.1 Configure using Jupyter Lab and new a Notebook: 
   ```bash
   jupyter lab
   ```
   4.2 Import packages:
   ```bash
   import ee
   import geemap
   ```
   4.3 Set the port number and then authenticate. Check the port number in Internet Properties and replace it with the corresponding local port number.
   ```bash
   geemap.set_proxy(7890)
   ee.Authenticate()
   ```
   4.4 Next, you will be redirected for authentication. Copy the token, paste it into the required field, and press Enter.  
   4.5 After successful authentication, proceed with Map visualization. If the map appears, it means the configuration was successful!
   ```bash
   Map = geemap.Map()
   Map
   ```
   

## Run the code

1. Activate your Conda environment: 
   ```bash
   conda activate gee
   ```
2. Update current environment
   ```bash
   conda env update --file environment.yml
   ```
2. Open Jupyter Notebook：
   ```bash
   jupyter notebook
   ```
3. Open `main.ipynb` and run

## Common issues
- **Geemap installation issues**：For more installation issues, please visit the official website for more information (https://developers.google.com/earth-engine/guides/python_install) 
