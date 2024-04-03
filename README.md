# DR classification model
This repository focuses  on the project structure rather than the accuracy of code implementation. It contains a PyTorch implementation of a deep learning model for image classification. In this README, we provide instructions for how to use the model.

# Model
This Python script models.py implements a factory design pattern for using different PyTorch classification models.

- `VGG19`
- `DensNet`
- `MyModel`

Each model is a PyTorch `nn.Module` and has a `predict()` method for making predictions on input data.


# How to Use
To use this script, simply run this command:

```bash
python main.py --input_CSV ${csv_path} --input_folder ${root_dir} --output_folder ${output_folder} --model 'DenseNet' --mode "train"

```
# Installation
1. Clone the repository: `git clone  https://github.com/SalahAli2018/SH.git`
2. Navigate to the repository directory: `cd SH`
3. Install the package: `pip install .`
4. Or use docker 
  build container
  ``` bash
  docker build -t diabetic_retinopathy_classifier .
  ```
  run  container
  
  ``` bash
   docker run -it diabetic_retinopathy_classifier
  ```
# Limitations

* It doesn't have many pre-processing functions
* it only has two models, but it's modular, and we can easily add any model as a class in `models.py`