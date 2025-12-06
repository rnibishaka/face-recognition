::: {style="color:red"}
# Face Recognition Pipeline (MediaPipe + LBPH)

This project implements a classical face recognition pipeline using:

-   **MediaPipe Face Mesh** → for face detection\
-   **OpenCV LBPH** → for feature-based face recognition

This project satisfies the "AI Without ML" assignment requirement.

------------------------------------------------------------------------

## 📂 Project Structure

project/ │── capture.py │── train.py │── predict.py │── dataset/ \#
Captured face images │── models/ │ ├── lbph_model.xml │ └──
label_map.json │── README.md

------------------------------------------------------------------------

## 🚀 1. Capture Face Images

Run:

    python capture.py

You will be asked:

    Enter your name:

-   Look at the camera.\
-   Press **Q** to stop capturing.\
-   Images are saved to:

```{=html}
<!-- -->
```
    dataset/<your_name>/

------------------------------------------------------------------------

## 🚀 2. Train the LBPH Model

Run:

    python train.py

This will generate:

-   `models/lbph_model.xml`\
-   `models/label_map.json`

------------------------------------------------------------------------

## 🚀 3. Run Face Recognition

Run:

    python predict.py

The camera window will show:

-   A **green rectangle** around the detected face\
-   The **predicted name**\
-   The **LBPH confidence score**

Press **Q** to quit.

------------------------------------------------------------------------

## 📋 Requirements

Install dependencies:

    pip install opencv-python mediapipe
    pip install opencv-contrib-python

------------------------------------------------------------------------

## 🎉 Notes

-   This pipeline works with **any number of people**.\
-   Just repeat **capture → train → predict** for each person.

------------------------------------------------------------------------

## 🔖 Tags

#face-recognition #opencv #mediapipe #LBPH
:::
