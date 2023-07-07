**Multi-View Dataset for Vehicle Detection in Complex Scenarios** is a dataset for instance segmentation tasks. It is used in the air detection industry.

The dataset consists of 9075 images with 87802 labeled objects belonging to 2 different classes including _small-vehicle_ and _large-vehicle_.

Images in the VSAI dataset have pixel-level instance segmentation annotations. Due to the nature of the instance segmentation task, it can be automatically transformed into a semantic segmentation (only one mask for every class) or object detection (bounding boxes for every object) tasks. There are 3703 (41% of the total) unlabeled images (i.e. without annotations). There are 3 splits in the dataset: _test_ (2315 images), _train_ (5240 images), and _val_ (1520 images). The dataset was released in 2022.

Here are the visualized examples for each of the 2 classes:

[Dataset classes](https://github.com/dataset-ninja/vsai/raw/main/visualizations/horizontal_grid.webm)
