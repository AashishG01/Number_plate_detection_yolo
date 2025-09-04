# Number Plate Detection using YOLOv8

This project uses a custom-trained YOLOv8 model to detect license plates in both images and videos. It includes a Jupyter Notebook detailing the model training process and a Streamlit application for an interactive user interface.

## Features

* **Real-time Detection:** Detects license plates from various sources like images and videos.
* **High Accuracy:** Utilizes the YOLOv8 object detection model, fine-tuned specifically for license plate recognition.
* **Interactive Web App:** A user-friendly Streamlit application to upload and process media files.
* **Detailed Training Process:** The `License_plate_detection.ipynb` notebook provides a step-by-step guide on how the model was trained.

## Demo

Here's a glimpse of the application detecting a license plate in an image and a video.

**Image Detection:**

[](images/sample_img.png)
[](images/sample_img2.png)
[](images/sample_img3.png)


**Video Detection:**



## Technologies Used

* Python
* PyTorch
* Ultralytics YOLOv8
* Streamlit
* OpenCV
* Pandas
* Matplotlib

## Setup and Installation

Follow these steps to set up the project locally.

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/AashishG01/Number_plate_detection_yolo](https://github.com/AashishG01/Number_plate_detection_yolo)
    cd Number_plate_detection_yolo
    ```

2.  **Create a virtual environment (optional but recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## Usage

### Streamlit Application

To run the interactive web application:

1.  Open the `yolo_applicaiton.py` file and update the path to the `best.pt` model weights to match its location on your system.

    ```python
    # yolo_applicaiton.py
    ...
    model = YOLO('path/to/your/best.pt') 
    ...
    ```

2.  Run the Streamlit app from your terminal:
    ```bash
    streamlit run yolo_applicaiton.py
    ```

3.  Open your web browser and navigate to the local URL provided by Streamlit to upload and process your files.

### Jupyter Notebook

The `License_plate_detection.ipynb` notebook contains the complete code for data preprocessing, model training, and evaluation. You can run it using Jupyter Notebook or JupyterLab to understand and replicate the training process.

## Project Structure

.
├── License_plate_detection.ipynb   # Jupyter Notebook for training the model
├── yolo_applicaiton.py             # Streamlit web application
├── best.pt                         # Trained YOLOv8 model weights
├── requirements.txt                # Python dependencies
├── images.jpeg                     # Sample image for testing
└── demo.mp4                        # Sample video for testing



## License

This project is unlicensed. You are free to use, modify, and distribute the code# Number_plate_detection_yolo
