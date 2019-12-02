# InHARD - Industrial Human Action Recognition Dataset  

## Objectives
This dataset is proposed

## Dataset description
The download link will be updated after reviewing process.  
**Reviewers**, please contact the main author for getting the link of the dataset.  

![dataset example](rsc/InHard_dataset.png)

## File naming convention  

## Modalities  
### Skeleton modality 
We used a “Combination Perception Neuron 32 Edition v2” motion sensor to capture the skeletal data delivered at a frequency of 120 Hz.  
Skeleton data comprises :
* the 3D locations (Tx, Ty and Tz) of 17 major body joints
* the 3 rotations around each axis (Rx, Ry and Rz)  
Skeleton data are saved into **BVH format** files and stored in the **Skeleton/ folder** of the InHARD dataset.  

<img src="rsc/Skeleton-joints-hierarchy.png" alt="Skeleton-joints-hierarchy" align="center">  

For manipulating BVH files, we recommand the [PyMO python library](https://github.com/omimo/PyMO/)

### Video modality
Each camera captures three different views of the same action. For each setup, two cameras were placed at the same height but at two different horizontal angles: -45° and +45° to capture both left and right sides. The third camera is placed on top of the subjects to capture the top view. 

* Camera 1 always observes top views and is displayed on the top left quarter of the RGB video. 
* Camera 2 observes left side views and is shown on the top right quarter of the RGB video. 
* Camera 3 observes right side views and is displayed on the bottom right quarter of the RGB video as shown in figure above

Files are stored in the **RGB/ folder** of the InHARD dataset.

## Action Classes
The list of **13 meta-actions** and **74 actions** classes are available in the [Action-Meta-action-list.xlsx](rsc/Action-Meta-action-list.xlsx) file


## Citation
For citing this work, please use:  
``` 
Available after reviewing process
```