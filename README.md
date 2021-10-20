# LP DAAC Cloud Data Access

## Description

This repository contains a series of Jupyter Notebooks, written in Python, demonstrating how to get started with NASA Earthdata in the cloud. The series covers the following topics:  
1. [Cloud Data Access in AWS](https://nbviewer.jupyter.org/github/amfriesz/lpdaac_cloud_data_access/blob/main/notebooks/Topic_1__AWS_Data_Access.ipynb)
2. [Cloud Optimized Data](https://nbviewer.jupyter.org/github/amfriesz/lpdaac_cloud_data_access/blob/main/notebooks/Topic_2__Cloud_Optimized_Data.ipynb)
3. [Data Discovery using STAC via NASA’s CMR-STAC API](https://nbviewer.jupyter.org/github/amfriesz/lpdaac_cloud_data_access/blob/main/notebooks/Topic_3__Data_Discovery_STAC_CMR-STAC_API.ipynb)
4. [Working with Cloud Data](https://nbviewer.jupyter.org/github/amfriesz/lpdaac_cloud_data_access/blob/main/notebooks/Topic_4__Data_Proximate_Compute.ipynb)

> **Note:** The notebooks found in this repository rely on packages, APIs, and specifications that are under active development. Changes to these dependencies can cause breaking changes to the code in the notebooks. The author(s) will endeavor to update the notebooks as changes are identified and/or encountered.

### Participation Options

[Launch Interactive Notebooks](https://openscapes.2i2c.cloud/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2Famfriesz%2Flpdaac_cloud_data_access&urlpath=lab%2Ftree%2Flpdaac_cloud_data_access%2F&branch=main)  

[View Static Notebooks](https://nbviewer.org/github/amfriesz/lpdaac_cloud_data_access/tree/main/notebooks/)  

## Assumptions

### User has an Earthdata Login Profile

An Earthdata Login account is required to access data, as well as discover restricted data, from the NASA Earthdata system. Thus, to access NASA data, you need Earthdata Login. Please visit <https://urs.earthdata.nasa.gov> to register and manage your Earthdata Login account. This account is free to create and only takes a moment to set up. 

### User has a Github Account (Required for the interactive notebooks, not for the static notebooks)

The interactive notebooks leverages the 2i2c Openscapes Jupyter Hub deploy on AWS in region us-west-2. This is a managed environment that requires authenication via Github credentials. To gain access follow the below steps:

1. [Sign up](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwiv9a-GmdnzAhW4l3IEHRAGAJkQFnoECAcQAQ&url=https%3A%2F%2Fgithub.com%2Fjoin&usg=AOvVaw0H9TK-nu7JfXaoNeNMgJEk) for a Github account
2. Add your Github username to the [2i2c Openscapes Jupyter Hub administrator document](https://docs.google.com/document/d/1dazKaqjFmGahsr-jVTDs4fBZJM1nd8UFG7fMGF5Gc7I/edit?usp=sharing)
3. Click the [Launch Interactive Notebooks](https://openscapes.2i2c.cloud/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2Famfriesz%2Flpdaac_cloud_data_access&urlpath=lab%2Ftree%2Flpdaac_cloud_data_access%2F&branch=main) link here, or above
4. Sign in using your Github username when prompted

### User is running notebook from within the AWS cloud region `us-west-2`

These notebooks were developed and tested within a managed JupyterHub deployed in the AWS region `us-west-2` using the [PANGEO](https://pangeo.io/) framework. Some notebooks include demonstration for accessing data assets directly in S3, which can incur a fee if the data is not accessed within the same cloud region as the data is store. The NASA and USGS data accessed in the notebooks are archived in the AWS region `us-west-2`.  

### User has a `netrc` file containing Earthdata Login credentials

You will need a netrc file containing your NASA Earthdata Login credentials in order to execute the notebooks. If you want to manually create your own netrc file, download the [.netrc file template](https://git.earthdata.nasa.gov/projects/LPDUR/repos/daac_data_download_python/browse/.netrc), add your credentials, and save to your home directory. If you want to use the python script to set up a netrc file but do not need to download any files, copy/clone/download the [EarthdataLoginSetup.py](https://git.earthdata.nasa.gov/projects/LPDUR/repos/daac_data_download_python/browse/EarthdataLoginSetup.py) script and execute it: `python EarthdataLoginSetup.py`. You will be prompted for your NASA Earthdata Login Username and Password, hit enter once you have submitted your credentials.  
 
