# Triple MNIST classifier

Classification of [triple MNIST](https://github.com/shaohua0116/MultiDigitMNIST) images using opencv, PyTorch, and Optuna.

**Solution steps:**

- **Digit cropper (opencv)**. By cropping the digits from images, I reduced the triple MNIST problem into simple MNIST
- Custom PyTorch **DataLoader** implementation
- **CNN model** for digits classification (trained on original MNIST dataset)
- **Image augmentations** (transforms.AutoAugment)
- **Automated fine-tuning of the model architecture**: you can specify value ranges and run Optuna trials for the following hyperparameters: number of layers, number of filters, activation function, learning rate, momentum, regularization
