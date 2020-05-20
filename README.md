# Installation

**1. Install Anaconda (Miniconda) from: [https://conda.io/miniconda.html](https://conda.io/miniconda.html).**
        
   * NOTE: If you are using a windows machine, you will need to open the anaconda terminal to execute the commands below.

&nbsp;&nbsp;


**2. Create and activate a conda environment:**
   * `conda create -n qgis_pyhat`
   * `conda activate qgis_pyhat`
   *  NOTE: If you want to restart installation, you should remove the `qgis_pyhat` environment and create a new one.
      * `conda deactivate`
      * `conda env remove -n qgis_pyhat`

&nbsp;&nbsp;


**3. To install the PyHAT library and dependencies:**
   * `conda config --add channels conda-forge`
   * `conda config --add channels usgs-astrogeology`
   * `conda install -c usgs-astrogeology pyhat`

&nbsp;&nbsp;


**4. To install QGIS:**
   * On windows: `conda install -c conda-forge qgis`
   * On linux: `conda install -c conda-forge qgis`
   * On OSX: `conda install -c conda-forge qgis`


&nbsp;&nbsp;


**5. Download the PyHAT QGIS plugin repo: <https://github.com/USGS-Astrogeology/pyhat_qgis.git>**
   * Click on the green "Clone or Download" button
   * Click "Download Zip"


&nbsp;&nbsp;


**6. Finish installation through QGIS:**

   * Run QGIS: `$ qgis`

   * On the bar at the top, click "Plugins > Manage and Install Plugins..."

   * On the left, select "Install from ZIP"
   ![Example of plugin menu](https://raw.githubusercontent.com/wiki/USGS-Astrogeology/PyHAT/images/plugin_menu.png)

   * Select the ZIP file downloaded in Step 5, hit "Install Plugin"

   * On the left, select "Installed"
   ![Enable plugin install](https://raw.githubusercontent.com/wiki/USGS-Astrogeology/PyHAT/images/plugin_installed.png)

   * You should see PyHAT listed as one of the plugins.

&nbsp;&nbsp;

# Running the plugin


* On the bar at the top in QGIS you should now see 'PyHAT'
* Click on it to see the two different menus for algorithms: M3, CRISM
* Make sure to have a layer (image) selected, and then click on any algorithm name
* You should now be able to view your new image in QGIS

&nbsp;&nbsp;

### NOTE: The images are saved on your computer, to change the path to somewhere you can find follow these steps: 
1. Click on PyHAT on the top menu
2. Click on 'Setup Outpath', a pop-up window should have appeared.
      ![Example of plugin menu](https://raw.githubusercontent.com/wiki/USGS-Astrogeology/PyHAT/images/plugin_outpath.png)
3. Enter the FULL path of where you want to store your images i.e. /home/your_username/Desktop/
4. Click okay and start going! 

&nbsp;&nbsp;

# Example Use Case

**1. Download this .tif to use as sample data: [M3_4030seg_L2_aristcrater.tif](https://github.com/USGS-Astrogeology/PyHAT/wiki/files/M3_4030seg_L2_aristcrater.tif)**

&nbsp;&nbsp;

**2. In QGIS, open the sample tif file as a layer**

 ![Input Layer](https://raw.githubusercontent.com/wiki/USGS-Astrogeology/PyHAT/images/input.png)

&nbsp;&nbsp;

**3. Select from the PyHAT option at the top:**

   * PyHAT > M3 > Pipe > bd1050

&nbsp;&nbsp;&nbsp;&nbsp;


**4. A new layer will have been placed in your view**

  ![Output Layer](https://raw.githubusercontent.com/wiki/USGS-Astrogeology/PyHAT/images/output.png)

