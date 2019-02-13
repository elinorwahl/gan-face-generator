# Generative Adversarial Network Face Generator

This is my implementation of a project to construct an adversarial neural network, and use it to generate photorealistic human
faces based on celebrity images. The original project notebook and requirements are part of Udacity's current Deep Learning 
course, which can be found [here](https://github.com/udacity/deep-learning) in the [face_generation](https://github.com/udacity/deep-learning/tree/master/face_generation) 
folder.

Generative adversarial networks are a kind of artificial intelligence that pits one neural network against another, in a form
of unsupervised machine learning. They are made of two deep neural networks, a generator and a discriminator. The generator
creates data, and the discriminator compares the generator's output to real-world data, like handwritten numbers, photographic 
images or music, and labels the generator's outputs real or fake in comparison. The discriminator's verdicts are then fed 
back to the generator, which uses them as guidance to make new attempts at generating data realistic enough to pass the 
discriminator's test.

As the two networks evolve, the generator learns to create more and more realistic outputs, and the discriminator learns to 
apply a more and more rigorous distinction between realistic and unrealistic inputs. Through this evolving competition, the 
two networks are ultimately meant to generate realistic data, without requiring supervision or direction. These GANs show a 
lot of potential for use in creative fields; they can be used to generate paintings, simulate voices, or craft images of 
chimeric animals that are a blend of multiple species.

### Usage

Clone the repository and navigate to the downloaded folder:
```
git clone https://github.com/elinorwahl/gan-face-generator.git
cd gan-face-generator
```

Using a GPU to run this project is very strongly recommended. If you plan to install TensorFlow with GPU support on your local 
machine, follow [this guide](https://www.tensorflow.org/install/) to install the necessary NVIDIA software on your system.
Some alternatives for web-hosted GPU use are [Amazon AWS](https://aws.amazon.com/hpc/) and [Crestle](https://www.crestle.com).
