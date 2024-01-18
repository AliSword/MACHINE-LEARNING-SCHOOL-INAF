Generative Adversarial Networks

It generate images of a certain kind  that don't exist by looking at the 
dataset.
You train at the same time 2 networks: the paiter and critic. One teach to 
the other (see slide 3).
But you need a good critic! It should train with the real image in order to
become better.
The painter is the generator and the critic is the discriminator.
Slide 8: CE: cross entropy. It minimize the error saying that the image is
fake.
The learning of generator and discriminator should go at the same level.
