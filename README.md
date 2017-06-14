This is our new multi-joint annotation for [EndoVis](https://endovissub-instrument.grand-challenge.org/) MICCAI Challenge dataset, which can be used for multi-instrument pose estimation.

# DATA 
EndoVis dataset is separated into training (in Tracking_Robotic_Training folder) and test data (in Tracking_Robotic_Testing folder): the training data includes four 45 seconds ex vivo video sequences of interventions, the test set is composed of 15 seconds additional video sequences for each of the training sequence, and two additional 1 minute recorded interventions. The frame resolution is 720 × 576 pixels.

# ANNOTATIONS
Compared to original annotation, our new annotation provides high quality annotation for multiple joints of the instrument. We manually labelled 940 frames of the training data (4479 frames) and 910 frames for the test data (4495 frames). The summery of annotation is listed below. 
#### Label / Frame Summery of the EndoVis Dataset
|            |   Seq 1  |   Seq 2  | Seq 3    | Seq 4    | Seq 5    | Seq 6    | Total      |
| ---------- | -------- | -------- | -------- | -------- | -------- | -------- | ---------- |
| Train Data | 210/1107 | 240/1125 | 252/1124 | 238/1123 |          |          | 940 / 4479 | 
| Test Data  | 80/370   | 76/375   | 76/375   | 76/375   | 301/1500 | 301/1500 | 910/4495   |

For each instrument, five joints including *LeftClasperPoint*, *RightClasperPoint*, *HeadPoint*, *ShaftPoint* and *EndPoint* joint are annotated, and the joint definitions in new annotation are illustrated in annotation_sample.png.


# CONTACT
When referring to these annotations, please contact us.
Citation details will be updated soon.

Xiaofei Du
Email: xiaofei.du.13@ucl.ac.uk
Dan Stoyanov
Email: danail.stoyanov@ucl.ac.uk


# License
MIT
