# Paper

* **Title**: All You Need Is A Good Init
* **Authors**: Dmytro Mishkin, Jiri Matas
* **Link**: https://arxiv.org/abs/1511.06422
* **Tags**: Neural Network, Initialization
* **Year**: ICLR 2016
* **Code**: https://github.com/ducha-aiki/LSUVinit

# Summary

* What
    - The paper describes an initialization method for deep sequential networks.
    - The idea it to keep variance of layer outputs equal to one through the network. 
* How
    - Initialize layer weights by Gaussian noise with unit variance. Then decompose them into orthonormal basis by QR or SVD-decomposition.  
    - From input to output, layer by layer, normalize the variance of output to one. 
* View
    - Single or only a few batch normalization during initialization, instead of every batch. 
    - Batch size used in initialization is not important.  

# Prerequisite

* Orthonormal initialize
    - Exact solutions to the nonlinear dynamics of learning in deep linear neural networks - Andrew M. Saxe, James L. McClelland, Surya Ganguli - https://arxiv.org/abs/1312.6120

# Implementation

* Official - https://github.com/ducha-aiki/LSUVinit
* Keras - https://github.com/ducha-aiki/LSUV-keras
