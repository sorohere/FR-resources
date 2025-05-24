# FR-resources
This repository provides two essential pre-trained models used in the face restoration pipeline, along with the main Face Restoration model. These models work together to enhance facial details and structure for improved restoration quality.

### Detection and Parsing Models
```
wget https://github.com/sorohere/FR-resources/releases/download/v.0.1.0/detection_Resnet50_Final.pth
wget https://github.com/sorohere/FR-resources/releases/download/v.0.1.0/parsing_parsenet.pth

echo "Downloaded face detection and parsing models successfully."
```

> `detection_Resnet50_Final.pth`: Face detection model – used to identify and crop face regions from images.
> `parsing_parsenet.pth`: Face parsing model – segments facial components such as eyes, nose, and mouth to guide restoration.

### Identity and Landmark Models
```
wget https://github.com/sorohere/FR-resources/releases/download/v.0.1.0/arcface_resnet18.pth -P pathToSave/here
wget https://github.com/sorohere/FR-resources/releases/download/v.0.1.0/FFHQ_eye_mouth_landmarks_512.pth -P pathToSave/here

echo "Downloaded ArcFace and landmark models successfully."
```
> `arcface_resnet18.pth`: Face recognition model – used to extract identity features.
> `FFHQ_eye_mouth_landmarks_512.pth`: Facial landmarks model – detects eye and mouth positions for accurate alignment and restoration.

### Face Restoration Model
```
wget https://github.com/sorohere/FR-resources/releases/download/v.0.1.0/StyleGAN2_512_Cmul1_FFHQ_B12G4_scratch_800k.pth -P pathToSave/here

echo "Downloaded face restoration model successfully."
```

> `StyleGAN2_512_Cmul1_FFHQ_B12G4_scratch_800k.pth`: StyleGAN2-based face restoration model – used to generate high-quality restored facial images.

### Face Restoration Model
```
wget https://github.com/sorohere/FR-resources/releases/download/v.0.2.0/FRv100ep.pth
wget https://github.com/sorohere/FR-resources/releases/download/v.0.2.0/FRv150ep.pth
wget https://github.com/sorohere/FR-resources/releases/download/v.0.2.0/FRv200ep.pth
wget https://github.com/sorohere/FR-resources/releases/download/v.0.2.0/FRv250ep.pth

echo "Downloaded Face Restoration model successfully."
```

> The `FRv*.pth` model is designed to restore low-quality or damaged face images by making use of structure-aware enhancements.
