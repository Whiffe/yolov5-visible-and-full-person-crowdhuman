##  Head & Visble Person Detection Model 

### Download model trained on crowd human using yolov5(m) architeture
Download Link:  [crowdhuman_vbody_yolov5m.pt](https://drive.google.com/file/d/1VJtrdE85Wc4xSZXqAPUkWABLResUYG8V/view?usp=sharing) 


<br/>

**Output (Crowd Human Model)**

![image](https://img-blog.csdnimg.cn/2bb374c4d17c4e049b9506b76ba6db6f.png)

<br/>



## Test

```bash
python detect.py --weights crowdhuman_vbody_yolov5m.pt --source _test/ --view-img

```
  
  
## Test (Only Person Class)

```bash
python3 detect.py --weights crowdhuman_vbody_yolov5m.pt --source _test/ --view-img  --person
```

  
## Test (Only Heads)

```bash
python3 detect.py --weights crowdhuman_vbody_yolov5m.pt --source _test/ --view-img  --heads
```
