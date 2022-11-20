# Learning Correction Filter via Degradation-Adaptive Regression for Blind Single Image Super-resolution

## Usage:

### Quick usage on testing dataset:  
To run on all images in <input_image_path>:

``` python main.py --input_dir <input_image_path> --gt_dir <gt_image_path> --scalr_factor 2 --scale_factor_downsampler 0.5 --output_dir <output_image_path> ```


``` python main.py --input_dir <input_image_path> --gt_dir <gt_image_path> --scalr_factor 4 --scale_factor_downsampler 0.25 --output_dir <output_image_path> ```

This will produce corrected LR images and SR results in the <output_image_path> folder. Note that GT images are only used to calculate PSNR, and does not participate in training.

example:

``` python main.py --input_dir LRx2 --gt_dir HR --scalr_factor 2 --scale_factor_downsampler 0.5 ```

This will produce corrected LR images and SR images in the results folder


### Quick usage on your data:  
To run on all images in <input_image_path>:

``` python main.py --input_dir <input_image_path> --scalr_factor 2 --scale_factor_downsampler 0.5 --output_dir  <output_image_path> ```


``` python main.py --input_dir <input_image_path> --scalr_factor 4 --scale_factor_downsampler 0.25 --output_dir  <output_image_path> ```

This will produce corrected LR images and SR results in the <output_image_path>  folder

The code is built on [KernelGAN](https://github.com/sefibk/KernelGAN) and [DualSR](https://github.com/memad73/DualSR). We thank the authors  for sharing the codes.
