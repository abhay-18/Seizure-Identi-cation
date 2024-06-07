# EEG-classification

This repo contains deep metric learning model for EEG signals classification for two classes (background, seizure).<br>
Dataset - <https://isip.piconepress.com/projects/tuh_eeg/html/downloads.shtml>


## How to run the code 

Step - 1
Create a virtual enviornment

```
python -m venv eeg_cls
```

Step - 2
Activate and install the requirements.txt file

```
source eeg_cls/bin/activate
```

```
pip install -r requirements.txt
```

Step - 4

Prepare the dataset

Please download from [https://www.isip.piconepress.com/projects/tuh_eeg/html/downloads.shtml](https://isip.piconepress.com/projects/tuh_eeg/html/downloads.shtml) 

For preprocessing the dataset, please refer to: `data_preparation`

Preprocessed Dataset should be in the form

```
  |-data
     |-train
        |-bckg
        |-seiz
     |-val
        |-bckg
        |-seiz
     |-test
        |-bckg
        |-seiz
```

The directory bckg and seiz contain fft images in .pkl format.
    
Step - 4
Run the model_cbam.ipynb cell by cell.



### References

- Roy, S., Asif, U., Tang, J., & Harrer, S. (2019). Machine learning for seizure type classification: setting the benchmark. *arXiv preprint arXiv:1902.01012*.

- Asif, U., Roy, S., Tang, J., & Harrer, S. (2019). Seizurenet: Multi-spectral deep feature learning for seizure type classification. *arXiv preprint arXiv:1903.03232*.
