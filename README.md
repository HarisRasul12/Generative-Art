# Style Transfer to Generative-Art

<img width="441" alt="Screen Shot 2022-03-13 at 3 43 29 PM" src="https://user-images.githubusercontent.com/66268214/158076278-dd9be202-afcf-4878-9fc7-6aefcec2ea24.png">



This project involves using a neural style transfer that takes the style of one image and the content of another to generate fused composite images. From there the outputs of the NST will be used a data set to feed into a generative adversarial network (GAN) to produce generated images similar to the fused compoistes.

The NST structure has followed models found online. We will be creating and modifying losses and accuracies of these models as well as changing major architecture componenets of the neural networks such as style weightings and  content weightings.

<img width="643" alt="Screen Shot 2022-03-13 at 3 45 34 PM" src="https://user-images.githubusercontent.com/66268214/158076335-cf072895-4b5b-49c0-b980-7df46b253d83.png"> 


The neural style transfer model is found in the follwoing 2 files NST.ipynb. WE tesed two different models to see which produces the better results and determined after tetsing that NST.ipynb had the better model. We determined this by changing style weightings and content weightings to get the results as seen above.


The orginal models for the two NST sructures can be found in the following:

Neural_Style_Transfer.ipynb:
LIGHT ON MATH MACHINE LEARNING, Intuitive Guide to Neural Style Transfer, An intuitive guide to exploring design choices and technicalities of neural style transfer networks, By Thushan Ganegedara
found here: https://towardsdatascience.com/light-on-math-machine-learning-intuitive-guide-to-neural-style-transfer-ef88e46697ee


NST.ipynb:
Sunghyun (psh01087) on GitHub
Found here: https://github.com/psh01087/style-transfer-pytorch



The original GANs archiecture used for development is found in the Gans_by_benji1123.ipynb file.The original GANS architecture by Ben Li found here: https://github.com/benji1123/gan/blob/master/dcgan_commented.py

This model is only used a base frame as of now and will need to be modified going forward as we need to create a data loader, tune style content hyperparamters, as well as GAN weightings based on the images passed in. However, cuurrently this architecture is able to generate random photos similar to the ones inputted into it.

The master GAN and NST architecture are found under the following:

MASTER_NST.ipynb

gan2.ipynb


The GANS and NST files were created with tuning hyper paramters such as style wieghtings, conent weightinsg - They are in the pipelkne created for the entire model.


<img width="787" alt="Screen Shot 2022-04-09 at 7 37 38 PM" src="https://user-images.githubusercontent.com/66268214/162595087-47835e2f-a16f-454f-8958-a7c74825c5db.png">


<img width="911" alt="Screen Shot 2022-04-09 at 6 17 56 AM" src="https://user-images.githubusercontent.com/66268214/162595092-21c19a1e-4061-4cba-89fa-11f639f9e39d.png">


