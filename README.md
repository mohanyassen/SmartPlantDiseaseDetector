# Data Folder README

## Folder structure

data/
├── public/
│   └── tomato/
│       ├── train/
│       ├── val/
│       └── test/
└── custom/
    └── phone_images/

## How to download public data
- PlantVillage tomato leaf dataset: [Kaggle link](https://www.kaggle.com/datasets/emmarex/plantdisease)
- Split into train/val/test as shown above

## Custom images
- Add phone images to `data/custom/phone_images/`
- Annotate bounding boxes if using detection mode

## Notes
- Images should be `.jpg` or `.png`
- For detection, create `.txt` label files per image
