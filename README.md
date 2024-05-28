# YOLOv8-Available-storage

### *Overview*
The YOLOv8 model is utilized to detect and localize areas where storage space is available in images or video streams.
The model is trained on a dataset containing images with labeled available storage areas. Once trained, 
the model can be used to identify and mark available storage spaces in real-time.

![alt text]( https://github.com/pahaht/YOLOv8-Available-storage/blob/main/images/as5.JPG)   


 ## Features 
- Fire detection using YOLOv8
- Real-time detection in video streams or images
-Real-time detection capability

### *Installation*
To install YOLOv8, please follow this link, which contains comprehensive 
documentation that will be beneficial to you: https://docs.ultralytics.com/

### *Dataset*
In this project, I used the Roboflow dataset https://universe.roboflow.com/test-shyto/available_storage

### *Training YOLOv8 based on Available storage*
-To understand well the training process follow this link :https://docs.ultralytics.com/modes/train/#why-choose-ultralytics-yolo-for-training
-To customize YOLOv8 for the Available storage dataset, run the following command : 

<pre><code>
from ultralytics import YOLO 
# Load the model.
model = YOLO('yolov8n.pt') 
# Training.
results = model.train(
   data="path to dataset\data.yaml',    
   imgsz=640,
   epochs=50,
   batch=8,)
</code></pre>

### *Loading available storage pre-trained model*  

<pre><code>
from ultralytics import YOLO
model = YOLO('weight_path'\available-storage.pt')
 </code></pre>

### *Detection of available storage*  

<pre><code>
display(Image.open('runs/detect/predict/as.jpg'))
  </code></pre>


