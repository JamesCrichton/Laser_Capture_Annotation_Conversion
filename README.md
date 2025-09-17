# Laser Capture Annotation Conversion
Converts annotations to xml format for high throughput laser dissection by Leica LMD6. 
Uses the py-lmd python package and notebooks modified from **https://mannlabs.github.io/py-lmd/**. 

# Getting started
If you don't have it already, download and install git (https://git-scm.com/downloads) and anaconda (https://www.anaconda.com/download). 

Open **anaconda prompt**, set directory, then run:

```
# Clone the github repo 
git clone https://github.com/JamesCrichton/Laser_Capture_Annotation_Conversion.git

# Build the necessary conda environment (this will be called "LMD_env")
conda env create -f "./Laser_Capture_Annotation_Conversion/LMD6_setup.yaml"

```
# Using 
After the conda environment has been reated (above), this just needs to be activated each time it's used:
```
conda activate LMD_env
```

Conversion of QuPath annotations from geojson format to xml is done in a Jupyter Notebook. 
Open this using the code below and follow the guidance in the notebook. 
Only the first cell should need editing to enter parameters for basic conversions. This is initially setup with paths to the demo file "Tissue_test_annotations.geojson"

```
Jupyter notebook "./Laser_Capture_Annotation_Conversion/QuPath annotation geojson xml conversion for LMD.ipynb"
```

When you're finished, the environment can be deactivated using

```
conda deactivate
```
