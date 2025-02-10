# Concurrent Geospatial Data for Supervising Invasive Species in Small and Dispersed Areas 
A geospatial data-driven approach to efficiently identify and manage invasive kudzu plant habitats using image recognition and classification techniques.

![Results](images/results.png)

## Overall Description
This project integrates geographic information systems to preprocess and integrate geospatial datasets, efficiently defining areas of interest (AOI) for kudzu habitats. The workflow utilizes Google Street View images and advanced techniques such as image classification and object detection, leveraging convolutional neural networks to confirm kudzu presence. This approach combines agriculture and technology to identify and manage invasive species habitats. By streamlining these processes, we reduce the need for extensive field trips and computational time, enhancing invasive species monitoring and management.


## Workflow
![Workflow of our proposed model](images/Workflow_diagram.png)

## Datasets
- Locations: [USGS Inhabit database](https://gis.usgs.gov/inhabit/)
- Training Dataset: [Kudzu Dataset](https://app.roboflow.com/test-mhm3s/kudzu-in-gsv/3) check if link works, should be redirected to roboflow

## Requirements
```python
PyTorch 1.7 + CUDA 10.1 + torchvision 0.8.2
TensorBoard 2.11
Numpy 1.22
tqdm 4.59
einops 0.4.1
matplotlib 3.6.20
```


## How to use this workflow
User Instructions for general users no need to be coders
1. Clone this repository.
2. Create a virtual environmnent with all the requirements.
4. Obtain a Google Maps API Key & a Roboflow API Key.
5. Run 1.StreetView.ipynb: this is the GSV Image Retrival process. Make sure to edit the variable `api_key = <YOUR_API_KEY_GOES_HERE>`
6. Run 2.YOLO.ipynb: this is the Kudzu Detection process. Make sure to edit the variable `api_key = <YOUR_API_KEY_GOES_HERE`

### Contact
Email: aclosatarres@wvstateu.edu

**Keywords:** geographic information systems, google street view (GSV), ecology, kudzu, workflow, object detection, convolutional neural networks
