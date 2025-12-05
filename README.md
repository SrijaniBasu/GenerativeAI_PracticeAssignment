# GenerativeAI_PracticeAssignment
Lab Exercise 1: GAN on MNIST

This repository contains a Jupyter notebook implementing and experimenting with a Generative Adversarial Network (GAN) trained on the MNIST handwritten digits dataset. The lab is organized as a guided exercise with partially completed code and “Your Tasks” sections for you to fill in and analyze.

## Notebook overview

Main sections:

1. **Introduction**  
   - Brief overview of GANs (generator vs discriminator) and the MNIST dataset.  
   - High-level training idea: generator tries to fool the discriminator, discriminator learns to distinguish real vs fake digits.

2. **Model Design**  
   - Definition of the generator and discriminator neural networks in PyTorch (`torch.nn`).  
   - Typical fully connected or simple convolutional architectures for MNIST-sized images.  
   - Use of appropriate activation functions and output shapes.

3. **Training Process**  
   - Loading MNIST using `torchvision.datasets.MNIST` and applying basic transforms.  
   - Creating `DataLoader` objects for batching.  
   - Defining optimizers (e.g., Adam or SGD) and loss functions (adversarial loss).  
   - Training loop that alternately updates discriminator and generator.  

4. **Your Tasks**  
   - **Task 1:** Examine the model code and answer conceptual/design questions about the generator and discriminator.  
   - **Task 2:** Examine the training code and answer questions about the training dynamics and loss behavior.  
   - **Task 3:** Write code to visualize generated digits using utilities like `torchvision.utils.make_grid` and `matplotlib`.  
   - **Task 4:** Analyze and discuss qualitative results: how realistic the generated digits look at epochs 10, 20, and 30.

## Requirements

The notebook is written in Python and uses PyTorch and related libraries.

Core dependencies:

- `python` (3.x)
- `torch`
- `torchvision`
- `matplotlib`

Typical installation (example):

pip install torch torchvision matplotlib


## How to run

1. **Clone or copy** the notebook into a working directory.
2. **Create and activate** a Python environment (optional but recommended).
3. **Install dependencies** as above.
4. **Launch Jupyter**:
5. Open `Lab_Exercise_1_GAN_on_MNIST_SrijaniBasu.ipynb` in the browser.
6. Run the cells in order:
- First run the import and setup cells.
- Then run the data-loading and model definition cells.
- Finally run the training cells and complete the “Your Tasks” markdown/code cells where indicated.

## Outputs and visualization

- During training, the notebook can:
- Print generator and discriminator losses per epoch.
- Save or display batches of generated digits at selected epochs (e.g., 10, 20, 30) using `make_grid` and `plt.imshow`.
- You are expected to:
- Implement or complete the visualization code (Task 3).
- Inspect generated images qualitatively and write a short discussion about training progress and image quality (Task 4).

## Educational goals

- Understand the basic GAN framework (generator vs discriminator) on a simple dataset (MNIST).
- Implement GAN components in PyTorch (models, losses, optimizers, and training loop).
- Practice reading and modifying research-style PyTorch code.
- Develop intuition for training stability and qualitative evaluation of generative models.
