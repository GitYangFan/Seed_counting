Count the seeds using Yolo v5 :)

# Quick start

## 1. train the model using customized dataset
python train.py --img 640 --epochs 100 --data 'data/seeds.yaml'

## 2. detect using pretrained model
python detect.py --weights 'runs/train/exp/weights/best.pt' --source 'data/images/test_jpg.rf.87287755d2299cbbf86e2c3f243bf591.jpg' --data 'data/seeds.yaml' --save-txt --hide-labels
