
### Generate TRT File/ Optimization
```
python export.py -o yolov7.onnx -e yolov7.trt 
python export.py -o yolov5.onnx -e yolov5.trt 
```
### Inference 
```shell
images
python trt.py -e yolov7.trt  -i src/1.jpg -o yolov7-1.jpg
python trt.py -e yolov5.trt  -i src/1.jpg -o yolov5-1.jpg

videos
python trt.py -e yolov7.trt  -v src/1.mp4 
python trt.py -e yolov5.trt  -v src/1.mp4


