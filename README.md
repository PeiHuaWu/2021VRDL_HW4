# 2021VRDL_HW4-Image super resolution

Train your model to reconstruct a high-resolution image from a low-resolution input.

## Environment
```
Ubuntu 16.04.5 LTS (GNU/Linux 4.15.0-39-generic x86_64)
```

## Requirements

To install the following modules:
```
!pip install -r requirement.txt
```

## Training

Before training the model, remember to put you training set and validation set in the folders `train_val/train` and `train_val/valid`

To train the model in the paper, run this command 
```
!git clone https://github.com/PeiHuaWu/2021VRDL_HW4.git
!python training.py --opt train_swinir_sr.json
```

## Testing

To evaluate my model on SWINIR, run this command
```
!python testing.py --model_path [path of the file final_weight.pth] --task classical_sr --scale 3 --folder_lq "datasets/testing_lr_images/testing_lr_images" 
```


## Files for downloading

You can also download the file here:

- [The file of final_weight.pth](https://drive.google.com/file/d/1DO2BSkoOHXJanNEXchLIwE5ovhh9h5S_/view?usp=sharing)
