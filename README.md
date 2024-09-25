# Spatial-Temporal-Channel Collaborative Feature Learning with Transformers for Infrared small target Detection

## Model
|![STC](./FIG/model.png)|
|:--:|
|*STC*|

## PR results on the ITSDT-15K and IRDST datasets


| ![pr](./Fig/PR.png) |
|:--:|
| *Ipr* |


## Datasets
### 1. Datasets are available at [IRDST](https://xzbai.buaa.edu.cn/datasets.html) and [ITSDT](https://www.scidb.cn/en/detail?dataSetId=de971a1898774dc5921b68793817916e&dataSetType=journal)

### 2. The COCO format need to convert to txt format.
``` python 
python utils_coco/coco_to_txt.py
```
### 3. The folder structure should look like this:
```
Dataset
├─coco_train.txt
├─coco_val.txt
├─annotations
├─images
│   ├─train
│   │   ├─data5
│   │   │   ├─0.bmp
│   │   │   ├─ ...
│   │   │   ├─2999.bmp
│   │   │   ├─ ...
│   │   ├─ ...
│   ├─test
│   │   ├─data6
│   │   │   ├─0.bmp
│   │   │   ├─ ...
│   │   │   ├─398.bmp
│   │   │   ├─ ...
│   │   ├─ ...
```
### 3. The class of dataset should write to a txt file. 
Such as model_data/classes.txt

## Train
The hyper-parameters are set in train.py
```python 
python tarin.py
```

## Evaluate
The hyper-parameters are set in vid_map_coco.py
```python 
python vid_map_coco.py
```

## Visualization
The hyper-parameters are setted in vid_predcit.py
```python 
python vid_predcit.py
```

## Reference
https://github.com/bubbliiiing/yolox-pytorch/
