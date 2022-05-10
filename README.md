# Adversarial-Attack

![image](https://user-images.githubusercontent.com/53564338/167610512-b39bde7c-733e-43f3-b896-fa18c7c3cc16.png)

This project entails the following;

	1 - The creation of an adversarial attack  of me(my images) trying resemble that of target(our case Emanuelle Macron)
	2 - The creation of a face mask mimicking the face of our target directly. Several image colors of face mask where used to make sure there is quite a good
variation in the face masks that were produced.

A number of 6 adversarial attacks were used from the Advertorch library https://advertorch-test.readthedocs.io/en/latest/advertorch/attacks.html. 

	1- MomentumIterativeAttack(Resnet - ImageNet)
	2- SparseL1DescentAttack(Resnet - ImageNet)
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

