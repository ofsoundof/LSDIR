# LSDIR: A Large Scale Dataset for Image Restoration

## How to use the dataset?
1. Download the dataset from the [LSDIR](https://ofsoundof.github.io/lsdir-data/) website or [Hugging Face](https://huggingface.co/ofsoundof/LSDIR).
2. Load the JSON file for the specific task.
   - `train.json`: for image restoration tasks based on synthetic data such as image denoising, real-world image super-resolution based on pure data synthesis, 
     JPEG compression artifact removal, Gaussian image deblurring, image demosaicking.
     - `path`: path to ground-truth images
   - `train_X2.json`: for X2 image super-resolution
     - `path_gt`: path to ground-truth images
     - `path_lq`: path to X2 low-resolution images
   - `train_X3.json`: for X3 image super-resolution
     - `path_gt`: path to ground-truth images
     - `path_lq`: path to X3 low-resolution images
   - `train_X4.json`: for X4 image super-resolution
     - `path_gt`: path to ground-truth images
     - `path_lq`: path to X4 low-resolution images
3. Write your own dataloader based on the loaded JSON file. (We will provide our dataloader soon.)

## Stay tuned!
The paper, code, and benchmark will be released soon.
