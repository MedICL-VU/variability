# Test-time Variability
Assessing Test-time Variability for Interactive 3D Medical Image Segmentation with Diverse Point Prompts
```
@article{li2023assessing,
  title={Assessing Test-time Variability for Interactive 3D Medical Image Segmentation with Diverse Point Prompts},
  author={Li, Hao and Liu, Han and Hu, Dewei and Wang, Jiacheng and Oguz, Ipek},
  journal={arXiv preprint arXiv:2311.07806},
  year={2023}
}
```
**Introduction**

Our code can be seamlessly integrated into any SAM-based or interactive methods for medical image segmentation.
We assessed the test-time variability using the pretrained [ProMISe](https://github.com/MedICL-VU/ProMISe), where the models can be found [here](https://drive.google.com/drive/folders/1Yol2tIaNYVve6JQ3osg2pjDRgwVeS-IF?usp=sharing).


**Installation**
```
conda create -n promise python=3.9
conda activate promise
(Optional): sudo install git
pip install torch==1.12.1+cu113 torchvision==0.13.1+cu113 --extra-index-url https://download.pytorch.org/whl/cu113 # install pytorch
pip install git+https://github.com/facebookresearch/segment-anything.git # install segment anything packages
pip install git+https://github.com/deepmind/surface-distance.git # for normalized surface dice (NSD) evaluation
pip install -r requirements.txt
```

**Datasets**

Here are the [datasets](https://drive.google.com/drive/folders/13uGNb2WQhSQcBQIUhnvYJere1LBYGDsW?usp=sharing) that we used in our experiments, which are modified based on the original datasets from [Medical Segmentation Decathlon](http://medicaldecathlon.com/). We used two public datasets, e.g. task 07 and 10 for pancreas and colon tumor segmentations, respectively. 

**Use**
```
python ./boundary_selection/boundary_selection.py
```

# contact
Please shot an email to hao.li.1@vanderbilt.edu for any questions and always happy to help! :).
