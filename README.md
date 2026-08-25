# NumPyVision

A from-scratch image processing project built with NumPy to understand how digital images are represented, manipulated, and processed at the pixel level.

NumPyVision applies core NumPy concepts to practical image-processing problems. The project focuses on understanding the numerical representation of images and implementing fundamental operations using array manipulation, indexing, slicing, broadcasting, vectorization, and mathematical operations.

The project is being developed progressively, starting with basic NumPy array operations and advancing toward fundamental computer vision techniques.

## Objectives

The main objectives of NumPyVision are to:

* Understand how digital images are represented as numerical arrays.
* Understand the structure of RGB image data.
* Manipulate individual pixels and image regions using NumPy.
* Apply mathematical operations directly to image data.
* Develop a strong understanding of NumPy indexing, slicing, reshaping, and broadcasting.
* Use vectorized operations instead of unnecessary Python loops.
* Implement fundamental image-processing techniques from scratch.
* Understand the numerical foundations behind basic computer vision operations.
* Build practical experience with NumPy in an AI/ML-oriented application.

## Project Roadmap

### Phase 1: Image Representation

* [x] Create an RGB image using a NumPy array
* [X] Understand image dimensions and color channels
* [X] Inspect `shape`, `ndim`, `size`, and `dtype`
* [X] Access individual pixels
* [X] Modify individual pixels
* [] Understand pixel intensity values

### Phase 2: Pixel Manipulation

* [ ] Modify RGB channels
* [ ] Select image regions using slicing
* [ ] Crop images
* [ ] Flip images
* [ ] Replace pixels based on conditions
* [ ] Apply basic color transformations

### Phase 3: Image Transformations

* [ ] Convert RGB images to grayscale
* [ ] Adjust brightness
* [ ] Adjust contrast
* [ ] Manipulate individual color channels
* [ ] Implement transformations using vectorized NumPy operations

### Phase 4: Efficient Numerical Processing

* [ ] Boolean indexing
* [ ] Broadcasting
* [ ] Vectorization
* [ ] Compare vectorized operations with Python loops
* [ ] Analyse computational efficiency

### Phase 5: Image Filters

* [ ] Understand image kernels
* [ ] Implement image blurring
* [ ] Implement sharpening
* [ ] Understand convolution
* [ ] Implement convolution using NumPy
* [ ] Implement basic edge detection

### Phase 6: Image Processing Pipeline

* [ ] Combine multiple image transformations
* [ ] Build reusable image-processing functions
* [ ] Create a simple image-processing pipeline
* [ ] Test the pipeline on different images
* [ ] Document results and limitations

## Image Representation

An RGB image can be represented as a three-dimensional NumPy array with the following structure:

```text
(height, width, channels)
```

For example:

```text
(1080, 1920, 3)
```

represents an image with:

* 1080 pixels in height
* 1920 pixels in width
* 3 color channels

The three channels represent:

```text
R — Red
G — Green
B — Blue
```

Each pixel therefore contains three numerical intensity values.

For example:

```text
[255, 0, 0]
```

represents a red pixel, while:

```text
[0, 255, 0]
```

represents a green pixel.

This representation allows image processing to be approached as numerical array manipulation.

## Technologies

### Primary

* Python
* NumPy
* Jupyter Notebook

### Supporting

* Matplotlib for visualization
* Pillow for image input and output
* Git and GitHub for version control

NumPy is used as the primary library for implementing the image-processing operations.

## Project Structure

```text
NumPyVision/
│
├── README.md
│
├── notebooks/
│   ├── 01_image_as_numpy_array.ipynb
│   ├── 02_pixel_manipulation.ipynb
│   ├── 03_image_transformations.ipynb
│   ├── 04_image_filters.ipynb
│   └── 05_edge_detection.ipynb
│
├── src/
│   └── ...
│
├── images/
│   ├── input/
│   └── output/
│
├── requirements.txt
│
└── .gitignore
```

The structure will evolve as the project develops.

## Learning Approach

The project follows a practical learning process:

1. Learn the underlying NumPy concept.
2. Experiment with small arrays.
3. Apply the concept to image data.
4. Observe and analyse the result.
5. Implement the operation using NumPy.
6. Compare different approaches where appropriate.
7. Document the concept and implementation.
8. Apply the knowledge to the next stage of the project.

The goal is to understand the underlying operations rather than relying on pre-built image-processing functions.

## Notebooks

The Jupyter notebooks document the technical development of the project.

Each notebook focuses on a specific concept and contains relevant explanations, implementations, experiments, outputs, and observations.

The notebooks are intended to demonstrate both the implementation and the reasoning behind each operation.

## Progress

| Milestone                 | Status      |
| ------------------------- | ----------- |
| Project setup             | In Progress |
| Image representation      | In Progress |
| Pixel manipulation        | Not Started |
| Image transformations     | Not Started |
| Vectorized processing     | Not Started |
| Image filters             | Not Started |
| Convolution               | Not Started |
| Edge detection            | Not Started |
| Image processing pipeline | Not Started |

This section will be updated as each milestone is completed.

## Skills Demonstrated

Upon completion, the project will demonstrate practical experience with:

* Python
* NumPy
* Multidimensional arrays
* Array indexing and slicing
* Array reshaping
* Boolean indexing
* Broadcasting
* Vectorization
* Numerical computation
* Image representation
* Pixel-level image processing
* Image transformations
* Convolution
* Image filtering
* Fundamental computer vision concepts
* Git and GitHub
* Technical documentation

## Future Improvements

Potential extensions to the project include:

* Image resizing
* Image rotation
* Additional convolution operations
* Advanced edge-detection techniques
* Histogram analysis
* Histogram-based image enhancement
* Performance benchmarking
* Additional computer vision algorithms
* Integration with machine-learning models

Future additions will be implemented after the underlying concepts have been studied and understood.

## Author

S Anirudh

This project is part of my development toward becoming an AI/ML Engineer, with an emphasis on building strong foundations in numerical computing, image processing, and practical machine-learning concepts.

## Project Status

Active development.

The project is being developed progressively as new NumPy and image-processing concepts are learned and implemented.
