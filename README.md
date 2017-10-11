# Densely Connected Convolutional Network (DenseNet)
paper: ["Densely Connected Convolutional Networks"](http://arxiv.org/abs/1608.06993)
This is the mxnet implement of DenseNet
You can git clone this project and do as follows:
* Prepare your image data and corresponding `.lst` file.
* Download pretrained model from

|Network 			   |     MXNet model|
|:-------------------: |:--------------:| 
|DenseNet-121 (k=32)   |[Google Drive (32.3MB)](https://drive.google.com/file/d/0ByXcv9gLjrVcb3NGb1JPa3ZFQUk/view)|
|DenseNet-169 (k=32)   |[Google Drive (57.3MB)](https://drive.google.com/file/d/0ByXcv9gLjrVcOWZJejlMOWZvZmc/view)|
|DenseNet-201 (k=32)   |[Google Drive (81.0MB)](https://drive.google.com/file/d/0ByXcv9gLjrVcUjF4MDBwZ3FQbkU/view)|
|DenseNet-161 (k=48)   |[Google Drive (115.7MB)](https://drive.google.com/file/d/0ByXcv9gLjrVcS0FwZ082SEtiUjQ/view)|

put the pretrained model under `DPN/models/` file.
* Change some configuration in `run_train.sh`, for example: `--epoch` and `--model` are corresponding to the pretrained model, `--data-train` is your train `.lst` file, `--image-train` is your train image file, `--save-result` is the train result you want to save, `--num-examples` is the number of your training data, `--save-name` is the name of final model.
* Run
```
run_train.sh
```