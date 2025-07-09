# DA-Net: Robust Crowd Counting in Dense Scenes

<img title="a title" src="results/78315csrnet 1.JPG">

This project presents **DA-Net (Density-Aware Network)**, a hybrid deep learning architecture for robust crowd counting. It addresses challenges like scale variations and occlusions by leveraging advanced techniques to accurately estimate crowd density and total counts in images.

## Key Features

- **EfficientNet-B5 Backbone:** For powerful feature extraction.

- **Feature Pyramid Network (FPN):** Enables multi-scale feature fusion.

- **Spatial Attention Mechanism:** Focuses on important crowd components.

- **Dilated Decoder:** Generates rich, semantic density maps without downsampling.

- **Custom Loss Function:** Combines MSE and Count MAE for accurate pixel-level and total count estimation.

## Performance

DA-Net achieved a Mean Absolute Error (MAE) of **20.99** on a challenging dataset, significantly outperforming baseline models like CSRNet and SegCrowdNet.

## Project Structure
```
crowd-counting-project/
├── notebooks/
│   ├── preprocess_data.ipynb   # Generates .npy density maps
│   ├── train_model.ipynb       # Trains the DA-Net model
│   └── test_model.ipynb        # Evaluates the trained model
├── .gitignore                  # Files to ignore in Git
├── requirements.txt            # Python dependencies
├── README.md                   # This file
└── LICENSE                     # Licensing information
```

## Getting Started

    Clone the repository: git clone https://github.com/vaibhavtripathi7/crowd-counting-project.git

    Install dependencies: pip install -r requirements.txt

    Download raw data: Obtain the dataset (e.g., ShanghaiTech) and place it in crowd_dataset folder.

    Preprocess data: Run notebooks/preprocess_data.ipynb to generate .npy files in processed_dataset folder.

    Train/Evaluate: Use notebooks/train_model.ipynb for training and notebooks/test_model.ipynb for evaluation.

## Detailed Documentation

For an in-depth understanding of the methodology, alternative architectures explored, experimental setup, and detailed analysis, please refer to the full project documentation:
 
<a href="https://github.com/Vaibhavtripathi7/Crowd-Counting/blob/main/doc/documentation.pdf">Documentation</a> 

## License

This project is licensed under the MIT License.

## Contact

Vaibhav tripathi

<a href="https://www.linkedin.com/in/vaibhav-tripathi-378634287/">Linkedin</a>  

Project Link: https://github.com/vaibhavtripathi7/Crowd-Counting