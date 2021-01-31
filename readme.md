# Instructions for running subsidence scripts
The following instructions will guide the user in running the subsidence scripts <br/>
The script subsidence_pipeline.py will create the vertical displacement files for every two pairs.
The script subsidence2timeseries.py will create images that show the cumulative vertical motion for a point that is closest to the point provided to the script.
All downloaded SAR data should be saved in a directory called 'input'. Scripts should be saved in a 'scripts' directory at the same level as input.
The subsidence_pipeline.py will create a directory called 'output' at the same level as the 'input' and the 'scripts' folder that contains IBEAM and NetCDF results
for vertical motion.
### Prerequisites
+ Ubuntu 20.04 LTS (otherwise you will only have SNAPHU 1.4.3 available. We need 2)
+ Python3 for ubuntu [anaconda 3](https://docs.anaconda.com/anaconda/install/linux/)
+ Snappy api for ubuntu [snappy api](https://senbox.atlassian.net/wiki/spaces/SNAP/pages/19300362/How+to+use+the+SNAP+API+from+Python).
+ Snaphu for Ubuntu 20.04 that you get by running the following from the CLI: sudo apt-get install -y snaphu
### Usage
+ Install all the prerequisites
+ Increase memory for SNAP using this [forum](https://forum.step.esa.int/t/increase-snappy-memory-beginner/6269)
+ Create an environment from the provided yaml file. For tips on how to do this use the [conda cheatsheet](https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf).
+ Activate your environment and in the next step, use this environment with the SNAP interface setup.
+ Configure python to use SNAP interface with [configure](https://senbox.atlassian.net/wiki/spaces/SNAP/pages/50855941/Configure+Python+to+use+the+SNAP-Python+snappy+interface#:~:text=Open%20the%20command%20line%20at,Line'%20from%20the%20Start%20menu.&text=Next%20you%20can%20call%20the,snappy%20folder%20should%20be%20created.)
+ In addition follow the advice to copy the 'snappy' module into your Python environment's 'site-packages' directory.This prevents problems with script hanging on import/output (IO) actions, such as writing to you SNAPHU directory.
+ Obtain SLC SAR IW (VV and VH) for a specific path from [Vertex](https://search.asf.alaska.edu/#/). Use their python script option for multiple downloads.

