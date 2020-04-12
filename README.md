# ROI_tools
# This is a Region of Interest (ROI) toolbox with the following 2 m-files:

# atlas_edit.m

Input atlas_roi in the command window to run. This allows you to obtain regions of interest anatomical brain atlas. 
You must know the number of the regions you wish to remove from or include in a new brain file or set of brain files.  
To obtain these region numbers for the AAL3 and the Harvard Oxford atlas see the Atlas_Regions.xls spreadsheet within the 
Research_Atlases folder.

The type of output depend on the following parameters:
‘ex’ : Allows you to exclude a set of numbered region from a standard brain atlas. Saves output as one nifti file.
‘inc-all’ :  Allows you to include a set of numbered regions from a standard brain atlas. Saves output as one nifti file.
‘inc’ :  Allows you to include a set of numbered regions from a standard brain atlas. Saves output as multiple nifti files. 

To edit the default parameters search for the line %% edit default parameters %%, and edit appropriate default parameters. 


# map_roi.m

Input map_roi in the command window to run. This allows you to obtain regions of interest from a statistical map. 
You must know the voxel level threshold, cluster size threshold (in voxels), and connectivity that you wish to use to 
define the clusters in your ROI.

The type of output depend on the following parameters:

‘cluster-index’ : outputs a single file (2 files if you indicate both positive and negative clusters) with a rank order 
number assigned to each cluster from largest to smallest. E.g. the largest cluster will have a number of 1 assigned to 
each voxel in the cluster. The output file name will have the voxel threshold, cluster threshold. and whether it is a 
positive (pos) or negative (neg).
‘clusters’: outputs a single file for each cluster with a rank order number assigned to each cluster from largest to smallest. 
E.g. the largest cluster will have a number of 1 assigned to each voxel in the cluster.  The output file name will have the 
voxel threshold, cluster threshold. the rank order cluster #, size of the cluster in voxels, whether it is positive (pos) or 
negative (neg), and the center of mass voxel. 

To edit the default parameters search for the line %% edit default parameters %%, and edit appropriate default parameters. 

