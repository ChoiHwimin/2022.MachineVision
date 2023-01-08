# 2022.MachineVision
2022년 머신비전시스템 강의


# Content
Camera Calibration, Filtering, Line Fitting, SIFT & Corner Detector, Homography, Transfer Learning, one-stage detector


# 환경
모든 과정은 colab 환경에서 진행하였습니다
tensorflow 및 keras를 사용하였습니다.


Camera Calibration
-----------
checkerboard가 찍힌 이미지들을 통해 corner를 검출 후 3차원 물체를 생성하는 과정입니다.


![mv1](https://user-images.githubusercontent.com/102031218/211219272-97a1bc2c-ab0f-4182-96a4-bb338611f067.jpg)


Filtering
-----------
원본 이미지에 노이즈를 추가한 후 average filter, gaussian filter, median filter를 적용하여 결과를 확인하는 과정입니다.


![mv2](https://user-images.githubusercontent.com/102031218/211219275-1d713c77-2aa1-4539-916a-7be106810903.jpg)
![mv3](https://user-images.githubusercontent.com/102031218/211219277-1a58aeba-144c-435b-be3f-9f1bbe92b70c.jpg)
![mv4](https://user-images.githubusercontent.com/102031218/211219278-8c94302c-4238-4a71-9a68-d1b55dc84825.jpg)

Line Fitting
-----------
RANSAC으로 도로에는 차선을 검출하는 Line fitting을 진행하는 과정입니다.


![mv5](https://user-images.githubusercontent.com/102031218/211219279-e49c9097-ae69-4424-868c-2e86d0f636ad.jpg)
![mv6](https://user-images.githubusercontent.com/102031218/211219280-f08a8ae1-9654-4d12-92e5-75ace6cd544c.jpg)


SIFT & Corner Detector
-----------
Harris corner detector로 코너를 검출을 진행합니다. 이후 두이미즈를 사용해 SIFT 를 통해 blob을 검출 후 matching을 수행하는 과정입니다.


![mv7](https://user-images.githubusercontent.com/102031218/211219282-83ddae38-b063-48ad-aaf6-7040b6b2e073.jpg)


![mv8](https://user-images.githubusercontent.com/102031218/211219284-3ab7ead4-8a3b-4762-8822-0b6dc2999a98.jpg)
![mv9](https://user-images.githubusercontent.com/102031218/211219285-4c19a6bf-a853-40b4-89fa-70ca034eddd3.jpg)


Homography
-----------
SVD를 사용하여 homography를 진행하고 합치는 과정입니다.


![mv10](https://user-images.githubusercontent.com/102031218/211219286-9c0d0a01-54d7-43d9-8421-ae29ddeb9e91.jpg)
![mv11](https://user-images.githubusercontent.com/102031218/211219287-de697290-7623-4d82-9a6d-2ee903b969f0.jpg)
![mv12](https://user-images.githubusercontent.com/102031218/211219289-7d21dae3-0723-4531-a200-30c2b729c106.jpg)

SIFT로 blob 검출을 토대로 Image Stitching을 진행합니다.


![mv13](https://user-images.githubusercontent.com/102031218/211219291-00ec37ec-e06d-46b6-9e98-b47994f6728a.jpg)
![mv14](https://user-images.githubusercontent.com/102031218/211219293-4e698862-7880-4cd8-b83f-6f600792a798.jpg)

Transfer Learning
-----------
Fashion Mnist와 CIFAR10 데이터셋을 사용하여 Lenet-5 와 VGG16을 통한 전이학습을 진행하였습니다.

Object Detection Step by step
-----------
one-stage detector 모델을 순차적으로 직접 만들어가며 진행합니다.


![mv15](https://user-images.githubusercontent.com/102031218/211219294-98fbf114-f580-41ce-b390-fecaf410d71d.jpg)
![mv16](https://user-images.githubusercontent.com/102031218/211219295-1b10c641-11e2-475f-afb0-752ec5a9aaf8.jpg)
![mv17](https://user-images.githubusercontent.com/102031218/211219296-70c013f3-4f2e-4042-a1cf-a6076d576b9d.jpg)
