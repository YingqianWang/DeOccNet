
### *"DeOccNet: Learning to See Through Foreground Occlusions in Light Fields". <a href="https://arxiv.org/pdf/1912.04459.pdf">WACV 2020</a>* <br><br>

### The project of *DeOccNet* can be downloaded  [*here*](https://wyqdatabase.s3-us-west-1.amazonaws.com/DeOccNet_codes.rar). 

### Requirements：

* python 3.7, cuda 9.2, cudnn 7.0, pytorch 1.3.0, torchvision 0.4.1;
* numpy 1.16.4+mkl, opencv-python 4.1.0.25 (only used for test);
* Matlab 2018a (for training and test data generation);

* Nvidia GPU (trained on RTX2080Ti, 11GB Memory);
* More than 500GB disk space to store training data (Here, an SSD is preferred);
* More than 32GB RAM is preferred since we do not perform cropping or resizing during test;

### Test:
* Prepare test LFs in folder ***Dataset***;
* Run ***GenerateDataForTest.m*** to generate test data;
* Execute ***test25.py*** or ***test75.py*** to implement DeOccNet for test;

### Train:
* Prepare training LFs in folder ***Dataset*** using the ***Mask Embedding*** approach;
* Run ***GenerateDataForTraining.m*** to generate training data (over 300 GB);
* Execute ***train.py*** to train DeOccNet on the generated data;

### The *Mask Embedding* Approach:
* Codes can be downloaded ***[here](https://wyqdatabase.s3-us-west-1.amazonaws.com/Mask_embedding.zip)***.
* Note: LFs in folders ***[LF_original_5](https://pan.baidu.com/s/1pvj-8b78yZelUwzLBXviIA)*** and ***[LF_original_15](https://pan.baidu.com/s/1cwRkSpl7qSysQb4nLNy2bw)*** can be downloaded via ***Baidu Drive***.

### Datasets:
* Synthetic datasets rendered using 3dsMax. ***[download](https://wyqdatabase.s3-us-west-1.amazonaws.com/Synscenes.zip)***
* Real-world datasets captured using cameras on a gantry. ***[download](https://wyqdatabase.s3-us-west-1.amazonaws.com/Realscenes.zip)***


### Citiations:
```
@InProceedings{DeOccNet,
     author = {Wang, Yingqian and Wu, Tianhao and Yang, Jungang and Wang, Longguang and An, Wei and Guo, Yulan},
      title = {De{O}cc{N}et: Learning to See Through Foreground Occlusions in Light Fields},
  booktitle = {Winter Conference on Applications of Computer Vision (WACV)},
      month = {Mar},
       year = {2020}
}
 ```

### Contact:
Please contact ***Yingqian Wang*** (wangyingqian16@nudt.edu.cn) for any question about this work. 

