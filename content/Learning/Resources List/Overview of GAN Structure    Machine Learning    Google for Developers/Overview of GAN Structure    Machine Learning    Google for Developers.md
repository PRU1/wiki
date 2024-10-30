---
Link: https://developers.google.com/machine-learning/gan/gan_structure
ee:
  - EE
---
A generative adversarial network (GAN) has two parts:

- The **generator** learns to generate plausible data. The generated instances become negative training examples for the discriminator.
- The **discriminator** learns to distinguish the generator's fake data from real data. The discriminator penalizes the generator for producing implausible results.

When training begins, the generator produces obviously fake data, and the discriminator quickly learns to tell that it's fake:

![[bad_gan.svg]]

As training progresses, the generator gets closer to producing output that can fool the discriminator:

![[ok_gan.svg]]

Finally, if generator training goes well, the discriminator gets worse at telling the difference between real and fake. It starts to classify fake data as real, and its accuracy decreases.

![[good_gan.svg]]

Here's a picture of the whole system:

![[gan_diagram.svg]]

Both the generator and the discriminator are neural networks. The generator output is connected directly to the discriminator input. Through [backpropagation](https://developers.google.com/machine-learning/glossary#backpropagation), the discriminator's classification provides a signal that the generator uses to update its weights.

Let's explain the pieces of this system in greater detail.