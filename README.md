# Forward_Looking_Under_Water_Mines_And_Debris_Sonar_dataset
This dataset is in **YOLO format** containing sonogram of  11 under water object classes. The dataset includes training, validation, and testing splits with corresponding annotations. During preprocessing, an additional Mine class was incorporated to support **underwater mine detection research, segmentation and bench marking**. 

## Features

- YOLO-compatible annotations
- 11 object categories
- Training, validation, and testing splits
- Ready for Ultralytics YOLO and other object detection frameworks
- Suitable for underwater robotics, autonomous underwater vehicles (AUVs), and marine perception research

## Dataset Structure

```text
Sonar_Dataset/
├── images/
│   ├── train/
│   ├── val/
│   └── test/
│
├── labels/
│   ├── train/
│   ├── val/
│   └── test/
│
└── data.yaml
```

## Object Classes

| ID | Class Name |
|---:|-------------|
| 0 | Mine |
| 1 | Can |
| 2 | Bottle |
| 3 | Drink Carton |
| 4 | Chain |
| 5 | Propeller |
| 6 | Tire |
| 7 | Hook |
| 8 | Valve |
| 9 | Shampoo Bottle |
| 10 | Standing Bottle |

## Annotation Format

Each label file follows the YOLO format:

```text
class_id x_center y_center width height
```

where all coordinates are normalized with respect to the image dimensions.

## Usage

This dataset can be used with:

- Ultralytics YOLO (v8, v9, v10, v11)
- RT-DETR
- Faster R-CNN
- Detectron2
- MMDetection
- Other object detection frameworks supporting YOLO annotations

## Applications

- Underwater object detection
- Underwater mine detection
- Sonar image analysis
- Deep learning research

## Kaggle Dataset

The complete dataset is also available on Kaggle:

**Forward-Looking Sonar Object Detection Dataset**  
https://www.kaggle.com/datasets/bhoumikchandrabagh/forward-looking-sonar-object-detection-dataset

## Citation

If you use this dataset in your research, please cite:

- This GitHub repository.
- The corresponding Kaggle dataset.
- The original dataset/publication from which the sonar images were obtained (if applicable).

## References

This dataset was prepared with reference to the following sources:

- [Marine Debris FLS Datasets](https://github.com/mvaldenegro/marine-debris-fls-datasets)
- [Mine Sonar Images Dataset](https://universe.roboflow.com/phan-quang-tuan/mine_sonar_images/dataset/1)

## License

Please refer to the repository license before using the dataset.
