# DL Project: Real-Time Partial Style Transfer

This is a project for NYU Deep Learning. For more details and reference, please refer to the project report in `docs` and the note in different notebooks.

### Implementation:
All the code are implemented using Google colab.

Installtation:

	! git clone https://github.com/pytorch/examples.git 
	! cp -r examples/fast_neural_style fast_neural_style
	! rm -r examples
	! python fast_neural_style/download_saved_models.py
	! rm -r saved_models.zip
	! mv -v saved_models/*.pth model

Models:
	To train your own style transfer, please refer to the [fast_neural_style](https://github.com/pytorch/examples/tree/master/fast_neural_style). For the joint model, the directory is [here](https://drive.google.com/drive/folders/1wDD0tb_XEsH0lpKYnod812UG0iImFnQ4)

Join Model:
	`join_model.ipynb` is use to join the segmentation model and style transfer model

Multiple object style transfer:
	Run `multi-object-partial-style.ipynb`, the result is listed as below

WebCamera:
	`webcam.ipynb` is use to simutanously generating the partial style transfer output video. Note that run on the colab may have huge delay, recommend the environment with full resource support

### Result:
Orginal Image             |Candy style             |Mosaic style             |Rain Princess style             |Udnie style             |Multiple object style transfer             |
:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:
<img src="https://github.com/samsh19/DL_project/blob/main/data/jennifer.jpeg?raw=true" width="200"/>  |  <img src="https://github.com/samsh19/DL_project/blob/main/result/candy.png?raw=true" width="200"/>  |  <img src="https://github.com/samsh19/DL_project/blob/main/result/mosaic.png?raw=true" width="200"/>  |  <img src="https://github.com/samsh19/DL_project/blob/main/result/rain_princess.png?raw=true" width="200"/>  |  <img src="https://github.com/samsh19/DL_project/blob/main/result/udnie.png?raw=true" width="200"/>  |  <img src="https://github.com/samsh19/DL_project/blob/main/result/multi_obj.png?raw=true" width="200"/>  |  



<!-- <p align = 'center'>
<img src = 'https://github.com/samsh19/ML_project/blob/main/data/compare_images/polor_bear_japan_paint_wave_compare.png?raw=true'>
</p>
From the left to right, the content image, style image, style transferred image, segmentation of the content image, and the outcome -->

Please feel free to leave a message [here](https://github.com/samsh19/DL_project/issues) if there is an issue.