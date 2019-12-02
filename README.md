# InHARD - Industrial Human Action Recognition Dataset  

## Objectives
This dataset is proposed

## Dataset description
The download link will be updated after reviewing process.  
**Reviewers**, please contact the main author for getting the link of the dataset.  


| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |



![dataset example](rsc/InHard_dataset.png)

## File naming convention  

## Modalities  
### Skeleton modality 
We used a “Combination Perception Neuron 32 Edition v2” motion sensor to capture the skeletal data delivered at a frequency of 120 Hz.  
Skeleton data comprises :
* the 3D locations (Tx, Ty and Tz) of 17 major body joints
* the 3 rotations around each axis (Rx, Ry and Rz)  
Skeleton data are saved into **BVH format** files and stored in the **Skeleton/ folder** of the InHARD dataset.  

<center><img src="rsc/Skeleton-joints-hierarchy.png" alt="Skeleton-joints-hierarchy">  </center>

For manipulating BVH files, we recommand the [PyMO python library](https://github.com/omimo/PyMO/)

### Video modality
Each camera captures three different views of the same action. For each setup, two cameras were placed at the same height but at two different horizontal angles: -45° and +45° to capture both left and right sides. The third camera is placed on top of the subjects to capture the top view. 

* Camera 1 always observes top views and is displayed on the top left quarter of the RGB video. 
* Camera 2 observes left side views and is shown on the top right quarter of the RGB video. 
* Camera 3 observes right side views and is displayed on the bottom right quarter of the RGB video as shown in figure above

Files are stored in the **RGB/ folder** of the InHARD dataset.

## Action Classes
The list of **13 meta-actions** and **74 actions** classes are available in the [Action-Meta-action-list.xlsx](rsc/Action-Meta-action-list.xlsx) file

Inside the InHARD.zip datatset, you will find the **InHARD.csv** file. It provides a dataframe with all info including Filename, Subject, Operation, Action low/high level label, Action start/end, Duration etc. in order to facilitate the dataset handling and use.  
See an extract below:  

|File_name|Subject|Operation|Action_label|Meta_action_number|Meta_action_label|Action_start_bvh_frame|Action_end_bvh_frame|Action_start_rgb_sec|Action_end_rgb_sec|Action_start_rgb_frame|Action_end_rgb_frame|Duration|
|-|-|-|-|-|-|-|-|-|-|-|-|
|0|D01_P01_R01_C01_C02_C03_OP|P01|OP010|[OP010] Consulter les Fiches|2|Consult sheets|323|1071|2.72|9.00|68|225|6.28|
|1|D01_P01_R01_C01_C02_C03_OP|P01|OP010|[OP010] Attraper le Lardon LARD|7|Picking left|1342|1528|11.28|12.84|282|321|1.56|
|2|D01_P01_R01_C01_C02_C03_OP|P01|OP010|[OP010] Placer LARD sur le Profil P360-1|12|Assemble system|1647|2247|13.84|18.88|346|472|5.04|
|3|D01_P01_R01_C01_C02_C03_OP|P01|OP010|[OP010] Attraper la Fixation FIXA1|6|Picking in front|2775|3028|23.32|25.44|583|636|2.12|
|4|D01_P01_R01_C01_C02_C03_OP|P01|OP010|[OP010] Placer FIXA1 sur LARD à 160mm|12|Assemble system|3151|3428|26.48|28.80|662|720|2.32|

## Experiments and performance metrics

S_train={P01_R01, P01_R03, P03_R01, P03_R03, P03_R04, P04_R02, P05_R03, P05_R04, P06_R01, P07_R01, P07_R02, P08_R02, P08_R04, P09_R01, P09_R03, P10_R01, P10_R02, P10_R03, P11_R02, P12_R01, P12_R02, P13_R02, P14_R01, P15_R01, P15_R02, P16_R02}  
S_val={P01_R02, P02_R01, P02_R02, P04_R01, P05_R01, P05_R02, P08_R01, P08_R03, P09_R02, P11_R01, P14_R02, P16_R01}  



## Citation
For citing this work, please use:  
``` 
Available after reviewing process
```