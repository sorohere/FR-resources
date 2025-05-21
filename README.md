# FR-resources
This repository provides two essential pre-trained models used in the face restoration pipeline, along with the main Face Restoration model. These models work together to enhance facial details and structure for improved restoration quality.

### Detection and Parsing Models
```
wget https://github.com/sorohere/FR-resources/releases/download/v.0.1.0/detection_Resnet50_Final.pth
wget https://github.com/sorohere/FR-resources/releases/download/v.0.1.0/parsing_parsenet.pth

echo "Downloaded face detection and parsing models successfully."
```

> Note:
> 
> `detection_Resnet50_Final.pth`: Face detection model – used to identify and crop face regions from images.
> `parsing_parsenet.pth`: Face parsing model – segments facial components such as eyes, nose, and mouth to guide restoration.

### Face Restoration Model
```
wget https://github.com/sorohere/FR-resources/releases/download/v.0.2.0/FR.pth

echo "Downloaded Face Restoration model successfully."
```

> The `FR.pth` model is designed to restore low-quality or damaged face images by making use of structure-aware enhancements.
