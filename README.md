# DL Project: Real-Time Partial Style Transfer

This is a project for NYU Deep Learning. For more details and reference, please refer to the project report in `docs` and the note in different notebooks.

### Implementation:
All the code is implemented using Google colab.

* Preparation:
	Installation

		! git clone https://github.com/pytorch/examples.git 
		! cp -r examples/fast_neural_style fast_neural_style
		! rm -r examples
		! python fast_neural_style/download_saved_models.py
		! rm -r saved_models.zip
		! mv -v saved_models/*.pth model

* Models:
	To train your own style transfer, please refer to the [fast_neural_style](https://github.com/pytorch/examples/tree/master/fast_neural_style). For the joint model, the directory is [here](https://drive.google.com/drive/folders/1wDD0tb_XEsH0lpKYnod812UG0iImFnQ4)

* Join Model:
	`join_model.ipynb` is used to join the segmentation model and style transfer model

* Multiple object style transfer:
	Run `multi-object-partial-style.ipynb`, the result is listed below

* WebCamera:
	`webcam.ipynb` is used to simultaneously generating the partial style transfer output video. Note that run on the colab may have a huge delay, recommend the environment with full resource support

### Result:
Original Image             |
:-------------------------:
![](https://github.com/samsh19/DL_project/blob/main/data/jennifer.jpeg?raw=true)  |

Original Image             |
:-------------------------:
<img src="https://github.com/samsh19/DL_project/blob/main/data/jennifer.jpeg?raw=true" alt="drawing" width="50"/>  |

Candy style             |Mosaic style             |Rain Princess style             |Udnie style             
:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:
![](https://github.com/samsh19/DL_project/blob/main/result/candy.png?raw=true)  |  ![](https://github.com/samsh19/DL_project/blob/main/result/mosaic.png?raw=true)  |  ![](https://github.com/samsh19/DL_project/blob/main/result/rain_princess.png?raw=true)  |  ![](https://github.com/samsh19/DL_project/blob/main/result/udnie.png?raw=true)  |

Multiple object style transfer             |
:-------------------------:
![](https://github.com/samsh19/DL_project/blob/main/result/multi_obj.png?raw=true)  |

Please feel free to leave a message [here](https://github.com/samsh19/DL_project/issues) if there is an issue.