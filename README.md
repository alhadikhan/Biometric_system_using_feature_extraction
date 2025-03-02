# Biometric System Using Feature Extraction

This project is a biometric identification system that leverages feature extraction techniques to process and match biometric data, such as fingerprints, iris scans, and facial images. Currently, it implements fingerprint matching using the SIFT (Scale-Invariant Feature Transform) algorithm and FLANN (Fast Library for Approximate Nearest Neighbors) matcher from OpenCV. Future updates will include iris scanning and face detection, with a modular design to preprocess and store features in a database.

## Features
- **Fingerprint Matching**: Extracts SIFT features from real fingerprints, matches them against altered fingerprints, and identifies the best match.
- **Preprocessing**: Loads and processes biometric images (currently fingerprints) in grayscale for feature extraction.
- **Feature Storage**: Saves precomputed features as `.npy` files to avoid redundant computation (database integration planned).
- **Scalable Design**: Built with extensibility in mind for adding iris scanning and face detection.
- **Efficient Matching**: Uses FLANN for fast descriptor matching with Lowe's ratio test for accuracy.

## Project Status
- **Current**: Fingerprint matching with SIFT and FLANN, using folder-based storage.
- **Future**: Add iris scanning, face detection, and database connectivity (e.g., SQLite, MongoDB).

## Prerequisites
- Python 3.x
- OpenCV (`cv2`) with SIFT support
- NumPy (`numpy`)
- Operating system with file system access (e.g., Linux, Windows)

Install dependencies:
```bash
pip install opencv-python numpy
