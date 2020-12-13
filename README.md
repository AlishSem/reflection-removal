# perceptual-reflection-removal



## Setup
  * Clone/Download this repo
  * `$ cd perceptual-reflection-removal`
  * `$ mkdir VGG_Model`
  * Download [VGG-19](http://www.vlfeat.org/matconvnet/pretrained/#downloading-the-pre-trained-models). Search `imagenet-vgg-verydeep-19` in this page and download `imagenet-vgg-verydeep-19.mat`. We need the pre-trained VGG-19 model for our hypercolumn input and feature loss
  * move the downloaded vgg model to folder `VGG_Model`

### Conda environment

A minimal conda environment to test the pretrained model is provided. (credit to @ironbar)

```
conda env create -f env.yml
```


## Testing

* Download pre-trained model [here](https://drive.google.com/open?id=1I9e2r_e0Ap6ds4MYRwoamUUlz6PzXPPj)
* `$ tar -xvzf pre-trained.tar.gz`
* this should extract the models into a newly created folder called `pre-trained`
* Change `test_path` (line 419) to your test image folder. If you want to test on the provided test images (e.g. in `./test_images/real/`), keep it as it is.
* test results can be found in `./test_results/`

Then, run

`$ python3 main.py --task pre-trained --is_training 0`


## Acknowledgement
Original model belongs to CeciliaVision (https://github.com/ceciliavision)


