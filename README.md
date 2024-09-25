# Vegan Vigilance: YOLOv8 Calorie Measurement for Raw Vegan Diet

This project utilizes **YOLOv8**, a state-of-the-art object detection model, to identify raw vegan food items from images and estimate their calorie content. The goal is to help users track their diet effortlessly by leveraging **artificial intelligence** (AI) and computer vision technologies. The project is built as a web application using **Flask** and provides real-time calorie measurement based on food image uploads.

## Features
- **AI-Powered Food Recognition**: Detects raw vegan food items from user-submitted images using YOLOv8 object detection.
- **Calorie Estimation**: Automatically estimates calorie content based on the detected food items and a pre-defined nutritional database.
- **Flask Web Application**: User-friendly web interface for uploading images and retrieving calorie information.
- **Pre-Trained Model**: Fine-tuned YOLOv8 model for high-accuracy food detection.

## Table of Contents
- [Features](#features)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Model](#model)
- [Contributing](#contributing)
- [License](#license)

## Project Structure
```
├── app.py                    # Main Flask application
├── README.md                 # Project documentation
├── best.pt                   # Pre-trained YOLOv8 model weights
├── Food and Calories - Sheet1.csv # Nutritional database (Food items and calories)
├── Input Image.jpg            # Sample input image
```

## Installation

### Prerequisites:
- Python 3.7+
- Flask
- PyTorch
- YOLOv8 (from Ultralytics)

### Steps:
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/vegan-vigilance.git
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Download the YOLOv8 pre-trained model and save it as `best.pt` in the root directory.

4. Run the application:
   ```bash
   python app.py
   ```

5. Access the web interface:
   Open your browser and navigate to `http://localhost:5000/`.

## Usage
1. Upload an image containing raw vegan food.
2. The YOLOv8 model will detect the food items in the image.
3. The app will return the calorie count based on the detected food items and the nutritional information from the CSV file.

## Model
The project uses a pre-trained YOLOv8 model for food recognition, which has been fine-tuned on a dataset of raw vegan foods to achieve over **90% accuracy**. The model weights are provided in the `best.pt` file.

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request or raise issues.
