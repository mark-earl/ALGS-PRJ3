# Seam Carving for PGMs and PPMs

This project implements a seam carving algorithm for images in the PGM (Portable Gray Map) and PPM (Portable Pixel Map) formats using Python. Seam carving is a technique used for content-aware image resizing, which intelligently removes or adds pixels in an image's least significant areas while preserving its most important features.

The algorithm implemented here allows you to resize images by either reducing or enlarging their dimensions while attempting to retain the important features and structures within the image.

## Getting Started

To use this project, you'll need the following prerequisites:
- Python (version 3.6 or above)
- Jupyter Notebook (optional but recommended for interactive usage)
- NumPy library (`numpy`)

## Installation

1. Clone or download this repository to your local machine.
2. Ensure you have Python installed. You can download it from [python.org](https://www.python.org/downloads/).
3. Install Jupyter Notebook using pip if you haven't already:
   ```
   pip install notebook
   ```
4. Install NumPy library:
   ```
   pip install numpy
   ```

## Usage

1. Launch Jupyter Notebook:
   ```
   jupyter notebook
   ```
2. Navigate to the directory where you cloned or downloaded this repository.
3. Open and run the `main.ipynb` notebook.
4. Follow the instructions within the notebook to load your image, specify the resizing parameters, and visualize the seam carving process.
5. Experiment with different resizing options and observe the results interactively.

## Supported Formats

This project supports the following image formats:
- PGM (Portable Gray Map): P2 (ASCII) and P5 (raw) formats
- PPM (Portable Pixel Map): P3 (ASCII) and P6 (raw) formats

## Implementation Details

The seam carving algorithm involves the following steps:
1. **Energy Calculation**: Compute the energy map of the image to identify the importance of each pixel.
2. **Seam Identification**: Find the least significant seam (a connected path of pixels) in the image using dynamic programming.
3. **Seam Removal or Duplication**: Remove or duplicate the identified seam to resize the image vertically or horizontally.

The notebook provides a step-by-step demonstration of these processes and allows you to visualize the effects of seam carving on your images.

## Examples

The `test` directory contains sample PGM and PPM images that you can use to test the seam carving algorithm.

## Contributing

Contributions are welcome! If you have suggestions for improvements or new features, please fork the repository and create a pull request. You can also open an issue if you encounter any bugs or have questions.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

This project is inspired by the original seam carving algorithm introduced by Shai Avidan and Ariel Shamir in their paper "Seam Carving for Content-Aware Image Resizing" (2007).

---

**Algorithms Classroom Project**

*The University of Akron, Spring 2024*

This project, developed by Mark P. Earl for a graduate-level Algorithms course at The University of Akron, implements a seam carving algorithm in Python for content-aware image resizing. Seam carving is a technique that intelligently resizes images while preserving important visual features. This implementation supports PGM and PPM image formats and includes an interactive Jupyter Notebook for visualization and experimentation.

*All Rights Reserved (c) Mark P. Earl 2024*
