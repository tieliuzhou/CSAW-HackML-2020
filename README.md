# CSAW-HackML-2020

```bash
├── data
    └── clean_validation_data.h5 // this is clean data to be used for designing your defense (validation)
├── models
    └── bd_net.h5
    └── bd_weights.h5
├── architecture.py
└── eval.py // this is the evaluation script
```

## I. Dependencies
   1. Python 3.6.9
   2. Keras 2.3.1
   3. Numpy 1.16.3
   4. Matplotlib 2.2.2
   5. H5py 2.9.0
   6. TensorFlow-gpu 1.15.2
   
## II. Validation Data
   Download the clean validation data from [here](https://drive.google.com/drive/folders/13o2ybRJ1BkGUvfmQEeZqDo1kskyFywab?usp=sharing) and store the data in `data/clean_validation_data.h5` directory.

## III. Evaluating the backdoored model
   1. To evaluate the backdoored model, execute `eval.py` by running
      `python3 eval.py <clean validation data directory> <model directory>`.
      
      E.g., `python3 eval.py data/clean_validation_data.h5  models/bd_net.h5`.
   3. Clean data classification accuracy on the provided validation dataset is 96.07 %.
