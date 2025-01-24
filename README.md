# Image Denoising with Autoencoder

## Overview
This project demonstrates an image denoising technique using a convolutional autoencoder. The model is trained on the MNIST dataset and can denoise grayscale images by removing random noise introduced into the input.

The project also includes functionality to process custom images, where you can provide a noisy image and receive a denoised output.

---

## Features
- **Autoencoder Architecture:** Utilizes convolutional layers for encoding and decoding.
- **Pre-trained Model:** The model is saved after training and loaded for inference to avoid retraining each time.
- **Custom Image Denoising:** Accepts any grayscale image, processes it, and outputs a denoised version.
- **Noise Addition:** Random noise is added to the MNIST dataset during training to simulate noisy inputs.

---

## Installation
1. Clone this repository:
   ```bash
   git clone <https://github.com/Kev-11/Denoisifier>
   ```
2. Navigate to the project directory:
   ```bash
   cd <project_directory>
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage
### Train the Model
If the autoencoder model is not already trained, the script will:
1. Load the MNIST dataset.
2. Add random noise to the dataset.
3. Train the autoencoder model.
4. Save the trained model to `autoencoder_model.h5`.

To train the model manually, run:
```bash
python image_denoising_autoencoder.py
```

### Denoise Custom Images
1. Place your noisy grayscale image in the desired directory.
2. Use the `denoise_image` function in the script by providing the image path:
   ```python
   denoise_image('path_to_your_image.png')
   ```
3. The script will display the original and denoised images side by side.

---

## Project Files
- **`image_denoising_autoencoder.py`:** The main script containing the model definition, training pipeline, and custom image denoising functionality.
- **`autoencoder_model.h5`:** Pre-trained model file (generated after training).
- **`requirements.txt`:** List of dependencies required for the project.

---

## Dependencies
- Python 3.x
- TensorFlow
- NumPy
- Matplotlib
- OpenCV

Install all dependencies using:
```bash
pip install -r requirements.txt
```

---

## Example
![image](https://github.com/user-attachments/assets/d0d32a0a-25a9-4a59-8915-abef489efaf5)


---

## Contributing
Contributions are welcome! Feel free to open an issue or submit a pull request.

---

## License
This project is licensed under the MIT License.

---

## Acknowledgments
- The MNIST dataset used in this project is provided by [Yann LeCun et al.](http://yann.lecun.com/exdb/mnist/).
- Inspired by the versatility of convolutional neural networks in image processing.

