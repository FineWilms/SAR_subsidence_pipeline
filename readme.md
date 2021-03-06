# Instructions for running subsidence scripts
The following instructions will guide the user in running the subsidence scripts <br/>
The script subsidence_pipeline.py will create the vertical displacement files for every two pairs.
The script subsidence2timeseries.py will create images that show the cumulative vertical motion for a point that is closest to the point provided to the script.
All downloaded SAR data should be saved in a directory called 'input'. Scripts should be saved in a 'scripts' directory at the same level as input.
The subsidence_pipeline.py will create a directory called 'output' at the same level as the 'input' and the 'scripts' folder that contains IBEAM and NetCDF results
for vertical motion.
### Prerequisites
+ Ubuntu 18.04 LTS
+ Python3 for ubuntu [anaconda 3](https://docs.anaconda.com/anaconda/install/linux/)
+ Snappy api for ubuntu [snappy api](https://senbox.atlassian.net/wiki/spaces/SNAP/pages/19300362/How+to+use+the+SNAP+API+from+Python).
+ Snaphu for linux [anaconda 3](https://step.esa.int/main/third-party-plugins-2/snaphu/)

### Usage
+ Install all the prerequisites
+ Increase memory for SNAP using this [forum](https://forum.step.esa.int/t/increase-snappy-memory-beginner/6269)
+ Create environments with the provided yaml files
+ Obtain SLC SAR IW (VV and VH) for a specific path from [Vertex](https://search.asf.alaska.edu/#/)
+ Activate the snap environment and run subsidence_pipeline.py from command line in Ubuntu
+ Activate the timeseries environment and run subsidence2timeseries.py
