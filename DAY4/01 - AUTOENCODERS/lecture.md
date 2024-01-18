Autoencoders

It is a type of algorithm with the purpose of learning an 'informative'
representation of the data that can be used for different applications.
You extract some information that can allow you to reconstruct a similar 
object (think for example to images).
For example as when you recognize someone from some features (for example a
friend of your mother).

How can we find these set of informative features that you need to reproduce
somenthing else well enough?
What does it mean well enough and informative?
Slide 11: encoder and decoder are NN. Decoder use output of encoder as input.
Autoencoders reconstruct inputs startinting from latent features.
You create an input starting from common feature (for example you cannot
create a spectra without any preliminary information).
Usually the latent feature as a lower dimension with respect to the initial
input.
It has also a computational advantage. It's faster reconstruct an image
starting from a lower dimensional input. That's called bottleneck.
In autoencoders loss functions (metric that gives you an indication of how 
good or bad the autoencoder was able to reconstruct the input observation)
is called reconstruction error.
Reconstruction error could be mean squared error, information matrix or 
something else. It depends by ypurself.
Slide 20: images built by different architechtures.
Slide 22: FFA: fit forward autoencoder
This approach is very valuable when you have large datasets.
You can aslo do data compression on latent features.

Denoising autoencoders:
(encoder and autoencoder have not the same weights.)
The encoder input is a noise image and the uotput a desnìnoise image.
The network is learning how the final image looks like and not how is the noise.
