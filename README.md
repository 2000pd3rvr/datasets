# Datasets Repository

This repository contains datasets for the SPAD for Vision project.

## Dataset Structure

Datasets are organized by type:
- `testmages__flatsurface/` - Flat surface test images
- `testmages__milkpurity/` - Milk purity test images
- `testmages__yolov3/` - YOLOv3 test images
- `testmages__yolov8/` - YOLOv8 test images
- `testmages_dino/` - DINO test images
- `testmages_spatiotemporal/` - Spatiotemporal test images
- `val_natural_material_detection/` - Natural material detection validation set

## Note

Due to GitHub's file size limitations, the actual dataset files are hosted on Hugging Face Hub:
- Organization: `mvplus`
- Dataset repositories: `mvplus/testmages__flatsurface`, `mvplus/testmages__milkpurity`, etc.

## Usage

Datasets can be downloaded from Hugging Face Hub using:
```python
from huggingface_hub import snapshot_download
snapshot_download(repo_id="mvplus/testmages__flatsurface", repo_type="dataset")
```

Or via the Hugging Face CLI:
```bash
huggingface-cli download mvplus/testmages__flatsurface --repo-type dataset
```
