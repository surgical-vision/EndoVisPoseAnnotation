# Multi-instrument multi-joint annotation for EndoVis'15 instrument subchallenge dataset
This is our new multi-joint annotation for [EndoVis'15](https://endovissub-instrument.grand-challenge.org/) MICCAI Challenge dataset, which can be used for multi-instrument pose estimation.

## Data 
After downloading the EndoVis'15 dataset, the dataset is separated into training (in *Tracking_Robotic_Training* folder) and test data (in *Tracking_Robotic_Testing* folder). The training data includes four 45 seconds ex vivo video sequences of interventions, the test set is composed of 15 seconds additional video sequences for each of the training sequence, and two additional 1 minute recorded interventions. The frame resolution is 720 × 576 pixels. Frames examples are shown below:

![data_sample](https://user-images.githubusercontent.com/6115717/27146869-b3761b1c-5132-11e7-81ff-2b841172b0a6.png)

## Annotations
Compared to original annotation, our new annotation provides high quality annotation for multiple joints of the instrument. We manually labelled 940 frames of the training data (4479 frames) and 910 frames for the test data (4495 frames). The summery of annotation is listed below:
#### Label / Frame Summery of the EndoVis Dataset
|            | Seq 1    | Seq 2    | Seq 3    | Seq 4    | Seq 5    | Seq 6    | Total      |
| ---------- | -------- | -------- | -------- | -------- | -------- | -------- | ---------- |
| Train Data | 210/1107 | 240/1125 | 252/1124 | 238/1123 |          |          | 940 / 4479 |
| Test Data  | 80/370   | 76/375   | 76/375   | 76/375   | 301/1500 | 301/1500 | 910/4495   |

For each instrument, five joints including *LeftClasperPoint*, *RightClasperPoint*, *HeadPoint*, *ShaftPoint* and *EndPoint* joint are annotated, and the joint definitions in new annotation are illustrated below:

![anno_sample](https://user-images.githubusercontent.com/6115717/27146913-e021bd60-5132-11e7-8c7a-4192bdeb8a5a.png)

The tool numbering in the annotation files helps distinguish between the scissor and clasper instrument (illustrated in the first figure). It follows the order below:
- Tool1: Right Clasper
- Tool2: Left Clasper
- Tool3: Right Scissor
- Tool4: Left Scissor

## Citation
If you use the annotation in your research, please use the following BibTeX entry.
```
@article{du2018articulated,
  title={Articulated multi-instrument 2-D pose estimation using fully convolutional networks},
  author={Du, Xiaofei and Kurmann, Thomas and Chang, Ping-Lin and Allan, Maximilian and Ourselin, Sebastien and Sznitman, Raphael and Kelly, John D and Stoyanov, Danail},
  journal={IEEE transactions on medical imaging},
  volume={37},
  number={5},
  pages={1276--1287},
  year={2018},
  publisher={IEEE}
}
```

## Contact
If you have any queries, please contact us.

Xiaofei Du: <xiaofei.du.13@ucl.ac.uk>

## License
MIT LICENCE
