

# Gearbox Fault Detection Using Continuous Wavelet Transform and Vision Transformer (ViT)

## Abstract

Managing the substantial volume of data generated by gearbox operations and the inherent complexities underscores the strategic advantage of employing deep learning methods. This study addresses fault detection in the gearbox using a Vision Transformer (ViT), whose images were prepared by continuous wavelet transformation. The dataset from the Open Energy Data Initiative (OEDI) serves as the foundation for our analysis. Data recorded by four vibration sensors, situated in the time domain and various operating loads, transform into two-dimensional images which, after some manipulations, are fed into a ViT, allowing us to tackle the classification challenge with 'Healthy' and 'Damaged' classes. Remarkably, we achieved an outstanding accuracy of 99.1554%, coupled with a reduction in the loss function to 0.040100. These results demonstrate the ViT's remarkable efficacy in detecting faults using images derived from signals recorded in the time domain.

## Repository Contents
- **![/dataloaders/README.md`](/dataloaders/README.md)**: Contains the source code for implementing the Continuous Wavelet Transform and Vision Transformer for gearbox fault detection.

- **![deeplearning/README.md`](/deeplearning/README.md)**: Contains the source code for Training the neural networks.

- **`/model`**: Containspre trained neural networks and results.

- **![/nets/README.md`](/nets/README.md)**: Contains the source code of the neural networks.

- **![/utils`](/utils)**: some functions and plotter.

## Dependencies

- Python  => 3.9
- Pytorch => 2.0
- NumPy   => 1.4
- Matplotlib
- Wavelet Transform Library (PyWavelets)

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yriyazi/GearBox_Fault_detection-ICEE2024.git
    ```

2. Download the dataset from [here](https://www.kaggle.com/datasets/brjapon/gearbox-fault-diagnosis) and place it in the appropriate directory.

3. Run the .\dataloader\splitter.py to generate the CWT images.
```bash
python splitter.py
```

4. Run the scripts to preprocess the data and train the model:

```bash
python train.py
```

## Usage

1. Navigate to the `/code` directory.

2. Execute the main script:

    ```bash
    python gearbox_fault_detection.py
    ```

3. Explore the results in the `/results` directory.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


## Citation

If you use this code or the FarsTail dataset in your research, please cite:

```
[Ali Asadian, Yassin Riyazi, and Seyyed Mossa Ayati*. 2024. " Gearbox Fault Detection Using Continuous Wavelet Transform and Vision Transformer (ViT)." ICEE, 2024, Page Numbers. DOI]
```

## Acknowledgments

- The Open Energy Data Initiative (OEDI) for providing the dataset.
- The contributors to the libraries and frameworks used in this project.

Feel free to reach out for any questions or collaborations!

---

*This README is generated with the assistance of ChatGPT.*
