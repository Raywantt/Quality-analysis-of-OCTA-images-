# Quality Analysis of OCTA Images

This repository contains the source code and resources for our project on assessing the gradability of OCTA images by analyzing the Foveal Avascular Zone (FAZ). The project leverages advanced image processing techniques and MATLAB code—specifically the Chan-Vese segmentation algorithm—to evaluate the quality of OCTA images.

## Overview

Optical Coherence Tomography Angiography (OCTA) images are essential for diagnosing retinal diseases. However, image quality can be compromised by issues like motion artifacts and noise. Our project focuses on automatically assessing image quality by analyzing the FAZ region, ensuring that only high-quality images are used for clinical analysis.

## Key Objectives

- **Image Quality Assessment:** Determine the gradability of OCTA images by analyzing the FAZ region.
- **Segmentation:** Utilize the Chan-Vese algorithm to accurately segment the FAZ.
- **Feature Extraction:** Measure key FAZ parameters (area, centroid, shape) to validate image quality.
- **Automation:** Develop a MATLAB-based pipeline for efficient and reproducible analysis.

## Methodology

1. **Pre-processing:** Enhance image contrast and reduce noise.
2. **Segmentation:** Apply the Chan-Vese segmentation algorithm to isolate the FAZ.
3. **Feature Extraction:** Compute geometric properties of the FAZ.
4. **Validation:** Assess the segmentation results to determine if the image is gradable.

## Results

- **Accuracy:** The algorithm achieved 72% accuracy on a 3x3 mm dataset and 69% on a 6x6 mm dataset.
- **Challenges:** Addressed issues include artifact detection and false positives in FAZ identification.
- **Enhancements:** Future improvements may involve integrating a broader field of view (12x12 mm) and additional anatomical markers.

## Installation & Requirements

- **MATLAB:** Ensure MATLAB is installed with the Image Processing Toolbox.
- **Dependencies:** No external libraries are required beyond MATLAB’s standard toolboxes.
- **Dataset:** Place your OCTA images in the directory specified in the main MATLAB script.

## Usage

1. **Setup:** Organize your OCTA dataset as per the instructions in the main script.
2. **Run:** Execute the main MATLAB script (e.g., `Demo.m`) to process the images.
3. **Output:** The script outputs segmentation results and computes FAZ metrics to assess image quality.

## Contributing

Contributions are welcome! If you have suggestions or improvements, please fork the repository and submit a pull request. For major changes, open an issue to discuss your ideas first.

## Acknowledgements

- **Project Team:** Adepu Ashvith, Aryan Toshniwal, Bhavesh Kumar Raktani, Param Shah, Warisha Basha, Raywant Beniwal.
- **Supervisors:** Dr. Shabnam Samima and Dr. Tauheed Ahmed.
- **Special Thanks:** To the MATLAB community and the developers behind the Chan-Vese segmentation algorithm.

## References

- Chan, T.F., & Vese, L.A. (2001). *Active contours without edges*. IEEE Transactions on Image Processing.
- Additional references are detailed in the [OCTA Report.pdf](./OCTA%20Report.pdf).
