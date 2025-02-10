# Concurrent Geospatial Data for Supervising Invasive Species in Small and Dispersed Areas 
A geospatial data-driven approach to efficiently identify and manage invasive kudzu plant habitats using object detection techniques.

![Results](images/results.png)

## Overall Description
This project integrates geographic information systems to preprocess and integrate geospatial datasets, efficiently defining areas of interest (AOI) for kudzu habitats. The workflow utilizes Google Street View images and advanced techniques such as image classification and object detection, leveraging convolutional neural networks to confirm kudzu presence. This approach combines agriculture and technology to identify and manage invasive species habitats. By streamlining these processes, we reduce the need for extensive field trips and computational time, enhancing invasive species monitoring and management.


## Workflow
![Workflow of our proposed model](images/workflow.png)

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
```
Ultralytics 8.3.53 🚀 Python-3.9.13 torch-2.2.2 CPU (Intel Core(TM) i5-8257U 1.40GHz)
Setup complete ✅ (8 CPUs, 16.0 GB RAM, 210.4/233.5 GB disk)

OS                  macOS-10.16-x86_64-i386-64bit
Environment         Darwin
Python              3.9.13
Install             pip
RAM                 16.00 GB
Disk                210.4/233.5 GB
CPU                 Intel Core(TM) i5-8257U 1.40GHz
CPU count           8
GPU                 None
GPU count           None
CUDA                None

numpy               ✅ 1.24.4>=1.23.0
numpy               ✅ 1.24.4<2.0.0; sys_platform == "darwin"
matplotlib          ✅ 3.5.2>=3.3.0
opencv-python       ✅ 4.6.0.66>=4.6.0
pillow              ✅ 9.2.0>=7.1.2
pyyaml              ✅ 6.0>=5.3.1
requests            ✅ 2.28.1>=2.23.0
scipy               ✅ 1.9.1>=1.4.1
torch               ✅ 2.2.2>=1.8.0
torch               ✅ 2.2.2!=2.4.0,>=1.8.0; sys_platform == "win32"
torchvision         ✅ 0.17.2>=0.9.0
tqdm                ✅ 4.64.1>=4.64.0
psutil              ✅ 5.9.0
py-cpuinfo          ✅ 9.0.0
pandas              ✅ 1.4.4>=1.1.4
seaborn             ✅ 0.11.2>=0.11.0
ultralytics-thop    ✅ 2.0.13>=2.0.0
```

## How to use this workflow
Steps:
1. Create a virtual environmnent with all the requirements.
2. Obtain a Google Maps API Key & a Roboflow API Key.
3. Run 1.StreetView.ipynb: this is the GSV Image Retrival process. Make sure to edit the variable `api_key = <YOUR_API_KEY_GOES_HERE>`
4. Run 2.YOLO.ipynb: this is the Kudzu Detection process. Make sure to edit the variable `api_key = <YOUR_API_KEY_GOES_HERE`

### Contact
Email: aclosatarres@wvstateu.edu

**Keywords:** geographic information systems, google street view (GSV), ecology, kudzu, workflow, object detection, convolutional neural networks
