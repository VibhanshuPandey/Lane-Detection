# Lane Detection Model using OpenCV

This project implements a lane detection model using OpenCV, a popular computer vision library. The model is designed to detect lane lines on the road from video or image inputs, which can be useful for various applications such as driver assistance systems, autonomous vehicles, and road safety analysis.

## Features

- Detects lane lines on the road from video or image inputs
- Processes the input using various image processing techniques like color selection, region of interest selection, Gaussian blurring, Canny edge detection, and Hough transform
- Renders the detected lane lines on the original input image or video frame
- Supports different video codecs and image formats

## Prerequisites

- Python
- OpenCV
- NumPy

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/vibhanshupandey/lane-detection.git
    ```

2. **Install the required dependencies:**

    ```bash
    pip install opencv-python numpy
    ```

## Usage

1. Navigate to the project directory:

    ```bash
    cd lane-detection
    ```

2. Run the lane detection script with the appropriate input:

    ```bash
    python lane_detection.py --input path/to/input_video.mp4
    ```

    or

    ```bash
    python lane_detection.py --input path/to/input_image.jpg
    ```

    The script will process the input video or image, detect the lane lines, and display the output with the detected lanes overlaid on the original input.

## Configuration

You can adjust various parameters in the `lane_detection.py` script to fine-tune the lane detection process:

- `region_of_interest`: Defines the region of interest in the frame where the lane lines are expected to be found.
- `canny_low_threshold` and `canny_high_threshold`: Thresholds for the Canny edge detection algorithm.
- `hough_lines_threshold`: Threshold for the Hough transform line detection algorithm.
- `line_color` and `line_thickness`: Customize the color and thickness of the rendered lane lines.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- The OpenCV team for developing and maintaining the computer vision library.
- Various online resources and tutorials for providing guidance on lane detection algorithms and techniques.
