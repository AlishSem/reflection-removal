# reflection-removal

Setup
•	Clone/Download this repo
•	$ cd reflection-removal
•	$ mkdir VGG_Model
•	Download VGG-19.
•	move the downloaded vgg model to folder VGG_Model
Conda environment
A minimal conda environment to test the pretrained model is as provided.
conda env create -f env.yml
Testing
•	Download pre-trained model here
•	$ tar -xvzf pre-trained.tar.gz
•	this should extract the models into a newly created folder called pre-trained
•	Change test_path (line 419) to your test image folder. If you want to test on the provided test images (e.g. in ./test_images/real/), keep it as it is.
•	test results can be found in ./test_results/
Then, run
$ python3 main.py --task pre-trained --is_training 0
Acknowledgement
Original model belongs to CeciliaVision
 
