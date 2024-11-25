# CUDA-based Edge Detection

## Project Overview
This project implements the Canny edge detection algorithm using CUDA to take advantage of GPU parallel processing capabilities. It processes grayscale images from an input directory, applies the edge detection using a CUDA kernel, and saves the results to an output directory. The goal of this implementation is to accelerate edge detection tasks, especially for large-scale image datasets.

## Project Structure
- **bin/**: Contains compiled binary or executable files. The executable files may have platform-specific extensions such as `.exe`.
  
- **data/**: Stores sample data in any format. If the original dataset is too large or can be generated through scripts, this folder may be left empty to avoid large downloads when only the code is needed.

- **src/**: Holds the source code organized in a logical structure.

- **README.md**: This file provides an overview of the project and its purpose, helping users understand its functionality and use cases.

- **Makefile**: Defines the steps to automatically build the project.

- **run.sh**: An optional script to execute the compiled program, with or without command-line arguments.

## Core Concepts
- CUDA programming for parallel computing
- Image processing techniques
- Edge detection methods
- Memory management within CUDA

## Supported Operating Systems
- Linux
- Windows (with appropriate adjustments)

## Supported CPU Architecture
- x86_64

## CUDA APIs Used
- `cudaMalloc()`
- `cudaMemcpy()`
- `cudaFree()`
- `cudaEventCreate()`
- `cudaEventRecord()`
- `cudaEventSynchronize()`
- `cudaEventElapsedTime()`

## Dependencies
- CUDA Toolkit
- OpenCV (version 4 or higher)

## Prerequisites
- Ensure the CUDA Toolkit is installed and your GPU supports CUDA.
- Install OpenCV via the appropriate package manager for your OS.

## Build and Execution
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. Install dependencies:
   - For OpenCV, use:
     ```bash
     sudo apt-get install libopencv-dev  # For Debian/Ubuntu
     ```

3. Compile the project:
   ```bash
   make all
   ```

4. Run the program:
   ```bash
   ./run.sh
   ```

5. The processed images will be saved in the `output/` directory.

## Sample Output

<img src="https://github.com/user-attachments/assets/5a43e30f-11e8-43ad-854f-1b526f35701c" width="720">
<img src="https://github.com/user-attachments/assets/1fa6b3cc-f751-413c-ad2b-353f7661c680" width="720">


