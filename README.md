# aayanmapara_nvidia_project

This project uses AI and Machine Learning to warn the user of any harmful mosquitos landing on the skin. This uses a re-trained model and works with the camera. The three mosquito species used in this dataset, all contain deadly diseases such as Zika and Malaria. This model can prevent people in third world countries from suffering, and even dying. The code used for this model is in the master branch. The dataset used is here: https://www.kaggle.com/datasets/naiborhujosua/mosquito-on-human-skin

The steps I took to use this model:

Step 1:
Download the dataset. The link for the dataset I used is above. Once, downloaded you only want to look at the data_splitting file. You can then delete all the other files.

Step 2: 
Transfer the dataset from your computer to the Jetson Nano data folder using the scp command on your host terminal. Once the files are transferred you have to rename "Train" to "train", "Test" to "test", and "Pred" to "val".

Step 3: 
Now you can train the model. I used 100 epochs but it takes a long time. If you need to stop the training you can always use the --resume flag. 

Step 4: Once the model is trained you can run some tests. This gives you a good idea as to how the model works, and how accurate it is.

Step 5: You can now use the camera and detectnet.py to test out the model in real life. I found that printing pictures of mosquitos on skin and showing them to the camera worked well!
