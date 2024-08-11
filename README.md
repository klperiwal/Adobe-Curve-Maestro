# Shape Detection Application

## Overview

The Shape Detection Application is a graphical user interface (GUI) tool that utilizes OpenCV and Tkinter to perform shape detection, symmetry detection, and curve completion on images. Users can upload an image to see detected shapes, check for symmetry, and observe completed curves in the provided images.

## Features

- **Shape Detection**: Identifies basic geometric shapes including triangles, squares, rectangles, pentagons, hexagons, and circles.
- **Symmetry Detection**: Highlights symmetrical contours and marks them with a label.
- **Curve Completion**: Fills gaps in curves and contours to complete shapes.

## Prerequisites

Ensure you have the following Python packages installed:

- `opencv-python`
- `numpy`
- `Pillow`
- `tkinter` (usually comes with Python's standard library)

You can install the required packages using pip:

```bash
pip install opencv-python numpy Pillow
```

## Usage

1. **Run the Application**: Execute the script to launch the GUI application.
   
   ```bash
   python shape_detection_app.py
   ```

2. **Upload an Image**:
   - Click the "Upload Image" button.
   - Select an image file (PNG, JPG, or JPEG) from your file system.

3. **View Results**:
   - The application will process the image and display three results:
     - **Detected Shapes**: Image with detected shapes outlined and labeled.
     - **Symmetry Detection**: Image highlighting contours with symmetry.
     - **Curve Completion**: Image showing completed curves and shapes.

4. **Text Labels**:
   - Information about detected shapes, symmetry detection status, and curve completion status will be displayed below the canvases.

## Code Explanation

- **`detect_shapes(image_path)`**: Detects and labels geometric shapes in the input image.
- **`find_symmetry(image_path)`**: Identifies and marks symmetrical contours in the input image.
- **`complete_curves(image_path)`**: Fills gaps in contours and curves in the input image.
- **`ShapeDetectionApp`**: The Tkinter GUI class that allows users to upload an image and view processed results.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- The OpenCV library for computer vision functionalities.
- Tkinter for creating the GUI interface.
- Pillow for image handling in the GUI.
