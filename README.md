# Setup Guide

Follow this guide to set up the environment and get started with the labs and projects.

---

## Step 1: Create a Folder

Start by creating a folder on your local machine to store the repository. For example:

```bash
mkdir TBMI26
cd TBMI26
```

---

## Step 2: Clone the Repository

Clone the repository from GitHub into the folder you just created:

```bash
git clone https://github.com/Berkay2002/TBMI26.git
```

Navigate into the repository folder:

```bash
cd TBMI26
```

---

## Step 3: Set Up the Environment

The repository includes multiple environment files to make dependency management easy. Choose the appropriate file based on your needs:

### 1. General Environment

For general-purpose tasks, use the `tbmi26_env.yml` file:

```bash
conda env create -n tbmi26 -f tbmi26_env.yml
```

Activate the environment:

```bash
conda activate tbmi26
```

### 2. TensorFlow Environment

For TensorFlow-specific tasks, use the `tbmi26_tf_env.yml` file:

```bash
conda env create -n tbmi26_tf -f tbmi26_tf_env.yml
```

Activate the environment:

```bash
conda activate tbmi26_tf
```

### 3. TensorFlow GPU Environment

For GPU-accelerated TensorFlow tasks, use the `tbmi26_tf_gpu_env.yml` file:

```bash
conda env create -n tbmi26_tf_gpu -f tbmi26_tf_gpu_env.yml
```

Activate the environment:

```bash
conda activate tbmi26_tf_gpu
```

---

### Note on A2: Deep Learning Lab

In the **A2: Deep Learning** lab, **Keras** will be used. Therefore, it is recommended to use either the `tbmi26_tf_env.yml` or the `tbmi26_tf_gpu_env.yml` file to create a kernel named `TBMI26-tf` or `TBMI26-tf-gpu` respectively. This ensures compatibility with all necessary deep learning dependencies.

---

## Step 4: Launch Jupyter Notebooks

Once the environment is activated, you can launch Jupyter Notebook to work on the labs and projects:

```bash
jupyter notebook
```

Navigate to the folder corresponding to the lab or task you want to work on, and open the desired notebook.

---

## Additional Notes

- Ensure that **Anaconda** or **Miniconda** is installed on your system.
- If you encounter issues with dependencies, update your `conda` version.
- For GPU support, verify that your system meets the requirements for TensorFlow GPU (e.g., CUDA and cuDNN compatibility).
