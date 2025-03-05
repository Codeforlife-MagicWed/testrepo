# 🐈 CatVTON: Concatenation Is All You Need for Virtual Try-On with Diffusion Models

## Setting Up the Environment
### 1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/catvton.git
  ```
### 2. Create and activate a conda environment:
  ```sh
cd <path_to_your_folder_project>
conda create -n catvton python==3.9.0
conda activate catvton
  ```
### 3. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
### 4. Download VITON-HD dataset:
  [VITON-HD dataset kaggle](https://www.kaggle.com/datasets/marquis03/high-resolution-viton-zalando-dataset)
## Inference
### 1. Data preparation
Once the datasets are downloaded, the folder structures should look like these:
   ```sh
├── VITON-HD
|   ├── test_pairs_paired.txt
│   ├── test
|   |   ├── image
│   │   │   ├── [000006_00.jpg | 000008_00.jpg | ...]
│   │   ├── cloth
│   │   │   ├── [000006_00.jpg | 000008_00.jpg | ...]
│   │   ├── agnostic-mask
│   │   │   ├── [000006_00_mask.png | 000008_00.png | ...]
...
   ```

We just use these for inference processing.

### 2. Inference on VTION-HD

