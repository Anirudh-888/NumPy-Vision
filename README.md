# NumPyVision

> A from-scratch image processing project built with NumPy to understand how digital images are represented, manipulated, transformed, and processed at the pixel level.

NumPyVision is a practical learning project focused on applying fundamental NumPy concepts to real image-processing problems.

The project begins with understanding how an image is represented as a multidimensional numerical array and progressively advances through pixel manipulation, geometric transformations, vectorized image processing, convolution, image filtering, edge detection, and a reusable image-processing pipeline.

The primary objective is to understand the underlying numerical operations behind image processing rather than relying on high-level image-processing functions.

---

## Table of Contents

- [Objectives](#objectives)
- [Project Philosophy](#project-philosophy)
- [Project Roadmap](#project-roadmap)
- [Current Progress](#current-progress)
- [Image Representation](#image-representation)
- [Image Array Structure](#image-array-structure)
- [Project Structure](#project-structure)
- [Notebook Overview](#notebook-overview)
- [Learning Approach](#learning-approach)
- [Technologies](#technologies)
- [Installation](#installation)
- [Usage](#usage)
- [Skills Demonstrated](#skills-demonstrated)
- [Future Improvements](#future-improvements)
- [Author](#author)
- [Project Status](#project-status)

---

## Objectives

The main objectives of NumPyVision are to:

- Understand how digital images are represented as numerical arrays.
- Understand the structure of RGB image data.
- Work with multidimensional NumPy arrays.
- Access and modify individual pixels.
- Manipulate image regions using indexing and slicing.
- Apply mathematical operations directly to image data.
- Understand image dimensions and axes.
- Perform geometric image transformations.
- Use Boolean masks for conditional image processing.
- Apply vectorized NumPy operations to images.
- Understand broadcasting in the context of image arrays.
- Compare vectorized operations with Python loops.
- Understand image kernels and convolution.
- Implement basic image filters from scratch.
- Implement fundamental edge-detection techniques.
- Build reusable image-processing operations.
- Develop practical foundations for computer vision and AI/ML.

---

## Project Philosophy

NumPyVision is designed as a **learning-by-building project**.

The focus is not simply on producing visually modified images. Every operation is intended to develop an understanding of the underlying NumPy concepts and numerical operations involved.

The project follows these principles:

- Understand the array structure before applying an operation.
- Learn the NumPy concept behind an image-processing technique.
- Experiment with small arrays when necessary.
- Apply the concept to real image data.
- Prefer vectorized operations over unnecessary Python loops.
- Understand the role of axes in multidimensional arrays.
- Observe and analyse the output of each transformation.
- Build progressively from simple operations to more advanced techniques.

The goal is to understand **why an operation works**, not just how to execute it.

---

# Project Roadmap

## Phase 1 — Image Representation

Understand how a digital image is represented using NumPy arrays.

- [x] Create and understand RGB arrays
- [x] Understand image dimensions
- [x] Understand RGB color channels
- [x] Inspect `shape`
- [x] Inspect `ndim`
- [x] Inspect `size`
- [x] Inspect `dtype`
- [x] Access individual pixels
- [x] Understand pixel intensity values
- [x] Visualize image arrays using Matplotlib

---

## Phase 2 — Pixel Manipulation and Basic Image Operations

Manipulate individual pixels and selected image regions using NumPy indexing, slicing, and mathematical operations.

- [x] Modify individual pixels
- [x] Modify RGB pixel values
- [x] Select image regions using slicing
- [x] Crop images
- [x] Modify selected image regions
- [x] Manipulate individual color channels
- [x] Replace pixel values
- [x] Apply mathematical operations to image regions
- [x] Increase image brightness
- [x] Decrease image brightness
- [x] Use `np.clip()` to control pixel intensity values

---

## Phase 3 — Geometric Image Transformations

Apply structural transformations by manipulating the spatial dimensions of image arrays.

- [x] Flip images horizontally
- [x] Flip images vertically
- [x] Transpose image arrays
- [x] Rotate images using NumPy operations
- [x] Perform 90-degree transformations
- [x] Perform 180-degree transformations

---

## Phase 4 — Vectorized Image Processing

Apply efficient NumPy operations to process complete images without manually iterating over individual pixels.

### RGB Channels

- [x] Extract the red channel
- [x] Extract the green channel
- [x] Extract the blue channel
- [x] Visualize individual color channels

### Grayscale Processing

- [x] Convert an RGB image to grayscale using numerical operations

### Boolean Masks and Thresholding

- [x] Create Boolean masks
- [x] Apply threshold conditions
- [x] Perform threshold-based filtering
- [x] Create binary images
- [x] Experiment with different threshold values

### Conditional Processing

- [x] Use `np.where()` for conditional image processing
- [ ] Apply Boolean masks directly to RGB images
- [ ] Use Boolean indexing to modify selected pixels
- [ ] Apply multiple conditions to create masks
- [ ] Perform color-based filtering

### Broadcasting and Vectorization

- [ ] Apply broadcasting to image arrays
- [ ] Perform vectorized image transformations
- [ ] Compare vectorized operations with Python loops
- [ ] Analyse basic computational efficiency

### Numerical Image Transformations

- [ ] Adjust image contrast
- [ ] Apply vectorized color transformations
- [ ] Apply numerical operations to complete images

---

## Phase 5 — Image Filters and Convolution

Understand how neighboring pixels can be mathematically combined using kernels.

- [ ] Understand image kernels
- [ ] Understand neighboring pixel operations
- [ ] Understand the concept of convolution
- [ ] Understand how a kernel moves across an image
- [ ] Implement basic convolution using NumPy
- [ ] Implement image blurring
- [ ] Implement image sharpening
- [ ] Experiment with custom kernels
- [ ] Analyse the effect of different kernels

---

## Phase 6 — Edge Detection

Use numerical operations and convolution to detect significant changes in image intensity.

- [ ] Understand edges as changes in pixel intensity
- [ ] Understand horizontal intensity changes
- [ ] Understand vertical intensity changes
- [ ] Understand edge-detection kernels
- [ ] Detect horizontal edges
- [ ] Detect vertical edges
- [ ] Combine edge information
- [ ] Implement basic edge detection using NumPy
- [ ] Visualize detected edges

---

## Phase 7 — Image Processing Pipeline

Combine the concepts developed throughout the project into a reusable image-processing workflow.

- [ ] Combine multiple image-processing operations
- [ ] Create reusable image-processing functions
- [ ] Organize operations into a processing pipeline
- [ ] Process different input images
- [ ] Test the pipeline on multiple images
- [ ] Compare results
- [ ] Document observations
- [ ] Document limitations

---

# Current Progress

| Phase | Status |
|---|---|
| Phase 1 — Image Representation | Completed |
| Phase 2 — Pixel Manipulation and Basic Operations | Completed |
| Phase 3 — Geometric Image Transformations | Completed |
| Phase 4 — Vectorized Image Processing | In Progress |
| Phase 5 — Image Filters and Convolution | Not Started |
| Phase 6 — Edge Detection | Not Started |
| Phase 7 — Image Processing Pipeline | Not Started |

---

# Image Representation

A digital RGB image can be represented as a three-dimensional NumPy array.

The general structure is:

```text
(height, width, channels)
```

For example:

```text
(1080, 1920, 3)
```

represents an image containing:

- **1080 pixels** in height
- **1920 pixels** in width
- **3 color channels**

The three channels represent:

```text
R → Red
G → Green
B → Blue
```

Each pixel contains numerical intensity values for the red, green, and blue channels.

For example:

```text
[255, 0, 0]
```

represents a red pixel.

```text
[0, 255, 0]
```

represents a green pixel.

```text
[0, 0, 255]
```

represents a blue pixel.

This numerical representation makes it possible to process images using multidimensional array operations.

---

# Image Array Structure

An RGB image can be accessed using:

```python
image[row, column, channel]
```

For example:

```python
image[100, 200, 0]
```

accesses the red-channel value of the pixel located at row `100` and column `200`.

The channel indexes are:

```text
0 → Red
1 → Green
2 → Blue
```

---

# Project Structure

```text
NumPyVision/
│
├── README.md
│
├── notebooks/
│   ├── 01_image_as_numpy_array.ipynb
│   ├── 02_pixel_manipulation.ipynb
│   ├── 03_image_transformations.ipynb
│   ├── 04_vectorized_image_processing.ipynb
│   ├── 05_image_filters.ipynb
│   ├── 06_edge_detection.ipynb
│   └── 07_image_processing_pipeline.ipynb
│
├── src/
│   └── ...
│
├── images/
│   ├── input/
│   │   └── Original input images
│   │
│   └── output/
│       └── Processed images
│
├── requirements.txt
│
└── .gitignore
```

The project structure may evolve as reusable functionality is moved from notebooks into the `src/` directory.

---

# Notebook Overview

## 01 — Image as a NumPy Array

Topics include:

- RGB arrays
- Image dimensions
- Color channels
- `shape`
- `ndim`
- `size`
- `dtype`
- Pixel values
- Pixel intensity
- Accessing individual pixels
- Image visualization

---

## 02 — Pixel Manipulation

Topics include:

- Pixel indexing
- Pixel modification
- RGB values
- Image slicing
- Region selection
- Cropping
- Region modification
- Channel manipulation
- Mathematical operations on pixels and regions
- Brightness adjustment
- Pixel intensity clipping

---

## 03 — Image Transformations

Topics include:

- Horizontal flipping
- Vertical flipping
- Image transposition
- 90-degree rotation
- 180-degree rotation

---

## 04 — Vectorized Image Processing

Topics include:

- RGB channel extraction
- Channel visualization
- Grayscale conversion
- Boolean masks
- Threshold filtering
- Binary images
- Conditional operations
- `np.where()`
- Boolean indexing
- Multiple conditions
- Color-based filtering
- Broadcasting
- Vectorization
- Contrast adjustment
- Vectorized transformations
- Vectorization versus Python loops
- Basic computational efficiency

---

## 05 — Image Filters and Convolution

Topics include:

- Image kernels
- Neighboring pixel operations
- Convolution
- Blur filters
- Sharpening filters
- Custom kernels

The objective is to understand how neighboring pixel values can be mathematically combined to transform an image.

---

## 06 — Edge Detection

Topics include:

- Intensity changes
- Horizontal edges
- Vertical edges
- Edge-detection kernels
- Combining edge information
- Basic edge detection using NumPy

---

## 07 — Image Processing Pipeline

Topics include:

- Combining image-processing operations
- Reusable functions
- Image-processing pipelines
- Multiple input images
- Testing
- Comparing results
- Limitations and observations

---

# Learning Approach

NumPyVision follows a practical learning process:

```text
Learn NumPy Concept
        ↓
Understand Array Operation
        ↓
Experiment with Small Arrays
        ↓
Apply to a Real Image
        ↓
Observe and Analyse the Result
        ↓
Improve the Implementation
        ↓
Apply the Concept in the Next Stage
```

The project emphasizes understanding rather than memorization.

The typical workflow is:

1. Learn the underlying NumPy concept.
2. Understand how it operates on arrays.
3. Experiment with a small example when necessary.
4. Apply it to real image data.
5. Observe the output.
6. Analyse what changed.
7. Implement the operation using NumPy.
8. Prefer vectorized operations when appropriate.
9. Document the implementation.
10. Move to the next concept.

---

# Technologies

## Primary Technologies

- Python
- NumPy
- Jupyter Notebook

## Supporting Technologies

- Matplotlib — Image visualization
- Pillow — Image input and output when required
- Git — Version control
- GitHub — Project hosting and documentation

NumPy is the primary library used for implementing the core image-processing operations.

---

# Installation

Clone the repository:

```bash
git clone <repository-url>
```

Navigate to the project directory:

```bash
cd NumPyVision
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

---

# Usage

The project is designed to be explored progressively.

Run the notebooks in numerical order:

```text
01 → Image Representation
          ↓
02 → Pixel Manipulation
          ↓
03 → Geometric Transformations
          ↓
04 → Vectorized Image Processing
          ↓
05 → Image Filters and Convolution
          ↓
06 → Edge Detection
          ↓
07 → Image Processing Pipeline
```

Each notebook documents:

- The concept being studied
- The NumPy operation involved
- The implementation
- The resulting output
- Observations from the experiment

---

# Skills Demonstrated

Upon completion, NumPyVision will demonstrate practical experience with:

## Python and NumPy

- Python programming
- NumPy arrays
- Multidimensional arrays
- Array indexing
- Array slicing
- Array axes
- Array operations

## Numerical Computing

- Vectorization
- Broadcasting
- Boolean indexing
- Conditional operations
- Numerical transformations

## Image Processing

- RGB image representation
- Pixel-level manipulation
- Image regions
- Image transformations
- Grayscale conversion
- Thresholding
- Binary images
- Image filtering
- Convolution
- Edge detection

## Software Development

- Jupyter Notebook documentation
- Git
- GitHub
- Project organization
- Technical documentation

---

# Future Improvements

Potential future extensions include:

- Image resizing
- Advanced image rotation
- Histogram analysis
- Histogram-based image enhancement
- Image normalization
- Advanced filtering techniques
- Additional convolution operations
- Advanced edge-detection techniques
- Performance benchmarking
- Additional computer vision algorithms
- Integration with machine-learning models

These improvements will be explored after completing the main project roadmap.

---

# Author

**S Anirudh**

This project is part of my development toward becoming an **AI/ML Engineer**.

NumPyVision focuses on building strong foundations in:

- Numerical computing
- NumPy
- Multidimensional arrays
- Image processing
- Vectorized computation
- Computer vision
- Machine learning foundations

The objective is not simply to complete an image-processing project, but to understand the numerical operations behind the techniques used when working with image data in artificial intelligence and machine learning.

---

# Project Status

**Active Development**

NumPyVision is being developed progressively as new concepts in NumPy, numerical computing, image processing, and computer vision are learned and implemented.