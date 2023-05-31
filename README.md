# VOC0712_FCOS
implement FCOS on VOC2007+2012 dataset

## training process
1，merge the VOC2007 and VOC2012 dataset, rename it as "VOC0712". For details you can refer to this repo https://github.com/YuwenXiong/py-R-FCN. I have merged the two datasets and put it in baidu netdisk for you to download directly. Download link: https://pan.baidu.com/s/1-kg3LEilM0IjlEinBgTdIA?pwd=fyaf. Make sure the merged dataset is under "./VOC0712"

2，download the resnet50 pretrained model. You can download it at "https://download.pytorch.org/models/resnet50-19c8e357.pth". Remember to rename it as 'resnet50.pth' and
put it under "./model/backbone"

3，run "train_voc.py" and then the model is saved in "./checkpoint"

## testing(evaluating) process 
1，make sure the trained model is under "./checkpoint"

2，run "eval_voc.py" to get the evaluating results. You may need to check the file path/name.

## detecting images
1，put your images to be detected in "./test_images"

2，run "detect.py" and the detecting result is saved in "./out_images"

