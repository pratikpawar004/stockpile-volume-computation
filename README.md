# Stockpile Volume Computation using 3D Point Cloud

This project performs stockpile volume estimation using 3D point cloud data with the help of Open3D and Python.

## Project Overview

The project workflow includes:

- Loading point cloud data
- Ground plane segmentation using RANSAC
- Noise removal
- Point cloud downsampling
- Delaunay triangulation
- Surface mesh generation
- Volume calculation

The final output is the estimated stockpile volume in cubic meters.

---

## Technologies Used

- Python
- Open3D
- NumPy
- SciPy
- Matplotlib

---

## Dataset

The project uses a `.ply` point cloud file containing 3D stockpile data.

---

## Workflow

### 1. Load Point Cloud
The point cloud data is loaded using Open3D.

### 2. Ground Segmentation
RANSAC plane segmentation is used to separate the ground plane from the stockpile.

### 3. Noise Removal
Statistical outlier removal is applied to clean the point cloud.

### 4. Downsampling
Voxel downsampling reduces point cloud density for faster processing.

### 5. Triangulation
Delaunay triangulation is used to create a surface mesh.

### 6. Volume Estimation
The volume under each triangle is calculated and summed to estimate the total stockpile volume.

---

## Screenshots

### Ground Plane Segmentation
<img width="1202" height="744" alt="Image" src="https://github.com/user-attachments/assets/e27fd36f-afe5-4444-8496-7ef79558d91c" />

### Cleaned Stockpile Point Cloud
<img width="1039" height="693" alt="Image" src="https://github.com/user-attachments/assets/a6ee6f8d-b59f-4b14-9dac-14b381395c68" />

### Triangulation Mesh
<img width="568" height="413" alt="Image" src="https://github.com/user-attachments/assets/8a628e5a-49d8-4e55-a7da-fbc708b4dab8" />

### Surface Mesh
<img width="1043" height="609" alt="Image" src="https://github.com/user-attachments/assets/07e5d47b-68ef-455a-b513-56ebb8e37bec" />

---

## Final Volume Output

Estimated stockpile volume: 0.1364 m3

---

## Installation

```bash
pip install open3d numpy scipy matplotlib
```

---

## Run Project

Open and run:

```bash
stockpile-volume-computation/
│
├── src/
│   ├── data/
│   │   └── stockpile.ply
│   └── stockpile_volume.ipynb
├── .gitignore
└── README.md
```

---

## Author

Pratik Pawar
