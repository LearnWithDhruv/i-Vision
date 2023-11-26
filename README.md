# I-Vision Walkthrough

## Steps
<br />
<b>Step 1.</b> Clone this repository: https://github.com/LearnWithDhruv
<br/><br/>
<b>Step 2.</b> Create a new virtual environment 
<pre>
python -m venv i-Vision
</pre> 
<br/>
<b>Step 3.</b> Activate your virtual environment
<pre>
source i-Vision/bin/activate # Linux
.\i-Vision\Scripts\activate # Windows 
</pre>
<br/>
<b>Step 4.</b> Install dependencies and add virtual environment to the Python Kernel
<pre>
python -m pip install --upgrade pip
pip install ipykernel
python -m ipykernel install --user --name=i-Visionobj
</pre>
<br/>
<b>Step 5.</b> Collect images using the Notebook <a href="https://github.com/LearnWithDhruv/Face_Recognition.ipynb">1. Image Collection.ipynb</a> - ensure you change the kernel to the virtual environment as shown below
<br/>
<b>Step 6.</b> Manually divide collected images into two folders train and test. So now all folders and annotations should be split between the following two folders. <br/>
\LearnWithDhruv\images\train<br />
\LearnWithDhruv\images.gz\test
<br/><br/>
<b>Step 7.</b> Begin training process by opening <a href="https://github.com/LearnWithDhruv/Face_Recognition.ipynb">2. Face_Recognition.ipynb</a>, this notebook will walk you through installing face Detection, making detections, saving and exporting your model. 
<br /><br/>
<b>Step 8.</b> During this process the Notebook will install a face Detection. You should ideally receive a notification indicating that the API has installed successfully at Step 8 with the last line stating OK.  
If not, resolve installation errors by referring to the <a href="https://github.com/LearnWithDhruv/README.md">Error Guide.md</a> in this folder.
<br /> <br/>
<br />
<b>Step 9.</b> You can optionally evaluate your model inside of Tensorboard. Once the model has been trained and you have run the evaluation command under Step 7. Navigate to the evaluation folder for your trained model e.g. 
<pre> cd Tensorlfow/workspace/models/my_ssd_mobnet/eval</pre> 
and open Tensorboard with the following command
<pre>tensorboard --logdir=. </pre>
Tensorboard will be accessible through your browser and you will be able to see metrics including mAP - mean Average Precision, and Recall.
<br />
