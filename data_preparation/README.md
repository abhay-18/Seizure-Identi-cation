# How to prepare data

Only support Python 3.

# Step 0: Download TUH data
Please download from [https://www.isip.piconepress.com/projects/tuh_eeg/html/downloads.shtml](https://isip.piconepress.com/projects/tuh_eeg/html/downloads.shtml) 

## Step 1: Build Data

Exemplary usage:                        
```
python3 data_preparation/build_data.py --input_data_dir [Path to Raw data] --save_data_dir [Path to data] 
```

## Step 2 Preprocess the data
Preprocess the data to generate fft images.

Exemplary usage:                        
```
python3 data_preparation/generate_fft_images.py --input_data_dir [Path to seizure type data] --preprocess_data_dir [Path to preprocessed seizure type data]
```
