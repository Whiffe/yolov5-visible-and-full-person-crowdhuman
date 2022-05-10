##  Head & Visble Person Detection Model 

### Download model trained on crowd human using yolov5(m) architeture
Download Link:  [crowdhuman_vbody_yolov5m.pt](https://drive.google.com/file/d/1VJtrdE85Wc4xSZXqAPUkWABLResUYG8V/view?usp=sharing) 


<br/>

**Output (Crowd Human Model)**

![image](https://img-blog.csdnimg.cn/2bb374c4d17c4e049b9506b76ba6db6f.png)

<br/>


## Install

```bash
git clone https://github.com/Whiffe/yolov5-visible-and-full-person-crowdhuman.git
cd yolov5
pip install -r requirements.txt 
pip install opencv-python-headless==4.1.2.30
mkdir -p /root/.config/Ultralytics
wget  https://ultralytics.com/assets/Arial.ttf -O /root/.config/Ultralytics/Arial.ttf

```

## Test

```bash
python ./detect.py --weights ./crowdhuman_vbody_yolov5m.pt --source ./1.jpeg --save-txt --save-conf


```
  
  
## Test (Only Visible Person Class)

```bash
python ./detect.py --weights ./crowdhuman_vbody_yolov5m.pt --source ./1.jpeg --save-txt --save-conf --classes 1


```

  
## Test (Only Heads)

```bash
python ./detect.py --weights ./crowdhuman_vbody_yolov5m.pt --source ./1.jpeg --save-txt --save-conf --classes 0

```
