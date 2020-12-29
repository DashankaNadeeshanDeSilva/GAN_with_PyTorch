**Generative Adversarial Networks (GANs)**

**GAN Architecture**

The basic GAN architecture is comprised of two separate models namely generator and discriminator. 

*Discriminator* : Typical image classifier is used and Convolutional neural networks are the mostly preferred classifier.

*Generator* : Learns to create fake data by incorporating feedback from the discriminator.

**How it works**

The generator creates fake data and the discriminator distinguishes between real and fake data. One can also say that generator is trying to fool the discriminator. In the training phase, the generator learns to become better with generating data that can fool the discriminator while the discriminator learns to tell how fake or real is the input data. As both models are implemented using deep neural networks, the parameters of both networks are tuned simultaneously and they both get better over time. Moreover, Feedback from the GAN output is used to train both generator and discriminator through backpropagation algorithm. The output of the discriminator is a probability of input is being a real. Higher the probability, more likely the input is from real data fed and lesser probability means fake data generated by the generator. When the discriminator is not being able to distinguish between fake and real, the probability output would be 0.5 which gives us the optimal solution. Furthermore, the loss function of a basic GAN architecture mainly based on two neural networks compete against each other which are differentiable with respect to their parameters and inputs.


This script contain vanilla GAN implemntation using Pytorch trained on the MNIST dataset, and learn to create hand-written digit images and MNIST-like generated images after training.

![image](https://github.com/DashankaNadeeshanDeSilva/GAN_with_PyTorch/blob/main/GAN%20generated%20MNIST%20images.png)



