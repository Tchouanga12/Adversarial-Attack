# Adversarial-Attack
As outlined in Szegedy (2014). In that paper, an adversarial example for a image classification NN is defined as “an imperceptible non-random perturbation to a test image” that changes the NN’s prediction.<br>
![image](https://user-images.githubusercontent.com/53564338/167613362-fd765756-a17d-4552-91f0-a6d2d5d08f0f.png)


![image](https://user-images.githubusercontent.com/53564338/167610512-b39bde7c-733e-43f3-b896-fa18c7c3cc16.png)

This project entails the following;

	1 - The creation of an adversarial attack  of me(my images) trying resemble that of target(our case Emanuelle Macron)
	2 - The creation of a face mask mimicking the face of our target directly. Several image colors of face mask where used to make sure there is quite a good

Diverse variations in the face masks were produced to diversify the creation the face color intensitifies and attacks.<br>
![image](https://user-images.githubusercontent.com/53564338/167612396-2cfb9b4a-7cb0-4917-b3f5-26efefd70ab6.png)

A number of 6 adversarial attacks were used from the Advertorch library https://advertorch-test.readthedocs.io/en/latest/advertorch/attacks.html. 

	1 -  MomentumIterativeAttack(Resnet - ImageNet)
	2 -  SparseL1DescentAttack(Resnet - ImageNet)
	3 - PGDAttack(Resnet - ImageNet)
	4 - MomentumIterativeAttack(Restnet - casia-webface)
	5 - SparseL1DescentAttack(Resnet - casia-webface)
	6 - PGDAttack(Resnet - casia-webface)

Creating adversarial attack on two face detection algorithms that is;
Face-mask resource: https://arxiv.org/pdf/2111.10759.pdf

	1. Resnet using Imagenet dataset
	2. Resnet using casia-webface dataset

A loss function was defined to calculate the distance between the set of me imgaes to target set of images.
![image](https://user-images.githubusercontent.com/53564338/167611439-839a86e4-c13c-4e3b-b963-c04ba1efe0a5.png)

**Note:** To request access to shared file: https://drive.google.com/file/d/1lSMbi6lwSk54wdDds9QYY8Gyw47snHBK/view?usp=sharing

	- You can easily create your me folder using a set of your own images.
	- you can make use of the provided target folder to experiement.

## Amelioration
Defining a mask as the variable you will optimize and then perform the gradient descent optimizing this variable which have already the right shape.

