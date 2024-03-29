# Consensus Focus for Object Detection

## Abstract
Ensemble methods utilize the knowledge generated in multiple instances under different domains to produce a joint decision for the same target. In AOI, ensembling the results from networks trained using the existing products with similar characteristics to the spot defects in a new production brings benefits such as a fast deployment without training as a temporary detection system, improved parameter sharing via knowledge vote or adjust the soft labels generated by a multi-source domain adaptation method. Thus, we present an ensemble method flexible for the previous applications thanks to the consensus focus for object detection based on weighted box fusion. In this sense, the algorithm removes bounding boxes with confidences below the class confidence gates;then, the weight box fusion constructs averages boxes from the filtered inferences and adjusts the contribution of each dataset via the consensus focus for object detection to produce high-quality bounding boxes based on the influence of each source dataset obtained through a heuristic analysis. The results showed the benefits of assigning weights to the bounding boxes from networks fed with source instances similar to the target in domain and task and reducing the impact of harmful sources without deleting them. 

**Keywords**: WBF, consensus focus, ensemble.

## Requirements

You can install the minimum requirements via pip or conda as follows:

**pip**
```
pip install -r requirements.txt
```

**Conda**
```
conda env create -f environment.yml 
conda activate Consensus_WBF1
```

You can also find all notebooks available in Google Colab. Please click on them, and you will find a link to see them.

## Description

### demo1.ipynb
This Jupyter notebook contains an example that uses offline inferences from three source networks to compute the consensus WBF.

## Implementation details
Our experiments were performed on a PC with an Intel(R) Core(TM) i5-10400F 2.90GHz CPU and an NVIDIA RTX 3060 GPU.

## Additional information about labels

Our datasets contain labels in Chinese, so we decided to translate them into English for research purposes. The chart below shows the changes we made.

| Defects | Original name |
| ------- | ------- |
| white crack | _bailiewen |
| standard chipping | _biaozhunbengque |
| standard crack | _biaozhunliewen |
| chamfer | _daojiao |
| multifaceted | _duocengmian  |
| crystallization | _jiejing |
| contour chipping | _lunkuobengque |
| superficial chipping | _mohubengque |
| ambiguity | _molengliangke |
| plane chipping | _pingmianbengque |
| light inking | _qianmo |
| triangular row | _sanjiaolie |
| bump | _tudian |
| fine cracks | _xixiaoliewen |
| impurities | _zazhi |
| chipping | bengque |
| abnormal chamfer | daojiaoyichang |
| crack | liewen |
| gas hole | qikong |
| stains | wuzi |