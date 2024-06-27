# Image_Project_Yolov10

1. Clone source YOLOv10 from Github
    !git clone https://github.com/THU-MIG/yolov10.git

2. Install the necessary libraries
    %cd yolov10
    !pip install -q -r requirements.txt
    !pip install -e

3. The weights of pre-trained models
    !wget https://github.com/THU-MIG/yolov10/releases/download/v1.1/yolov10n.pt

4. Model initialization
    from ultralytics import YOLOv10

    MODEL_PATH = "yolov10n.pt"
    model = YOLOv10(MODEL_PATH)

5. Predict
    IMG_PATH = " "
    result_img = model(source = IMG_PATH, save = True)

    VIDEO_PATH = " "
    result_videp = model(source = VIDEO_PATH, save = True)