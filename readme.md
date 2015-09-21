Neural Networks - Formulae Collection
=====================================

This is my personal collection of formulae in the field of neural networks. Where I felt the need for it I also added explanations and derivations. I started it in preparation to my exam on the neural nets at Karlsruhe Institute of Technology (KIT). Even so the content is similar to the course topics it is neither limited to it nor guaranteed to cover it completely. __These are not official lecture notes and may contain errors and lag completeness.__

Corrections, supplements (or wishes for it) and links to good sources/ papers are very welcome. Just mail me to marvin.ritter@gmail.com or create a ticket/pull request.

Todo's
------
- Overview off network architectures (feed forward networks: perceptron, MLP, DNN; shared parameters: DA, TDNN, CNN; recurrent networks: Hopfield nets, BM, RBM, RNN)
	perceptron, ff (MLP-TDNN, CNN), recurrent (Hopfield, BM, RBM)
- SVM
- Optimal Brain Damage, Optimal Brain Surgeon
- Cascade Correlation
- Meiosis
- Section on splitting the training data into training set, validation set, development set, test set, ...
- Hyperparamaters \Theta (list of examples, how to choose/train them?)
- Explain overfitting and underfitting (what is it, how to detect, how to prevent)
- Quickprop (Pattern Recognition 6.9.3)

- Conjugate gradient method
- What is the Schwarz Criterion for k-Means
- Least squares revisited for Perceptrons, see cs229-notes1.pdf for 

- laterale Verbindungen/latente Variable
- Overview of Pattern recognition (graphic + examples)
- Compare BGD, SGD and SGD with minibatches
- Derivation of the formular for the capaicty in Hopfield nets
- Chapter on common datasets/ benchmarks
	- MNIST
	- CIFAR-10: 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images. 

Out of scope (at least for now)
-------------------------------
- DBM (deterministic Boltzmann machine)
- Hebbian learning rule
- What is Curriculum Learning?
- L_1 vs L_2 regularization, feature selection
- AdaBoost

Open Questions
--------------
- Backpropagation requires the activation function to be differentiable. How can be use non differentiable activation functions, e. g. step function, ReLu
- Is LBG better than k-Means? In LBG in could check the loss function value for 1,2,4,...,k manually, k-Means should be faster.
- What should I learn from slide V07 page 23
- If we run a 5-layer DA forward and backward on a speech signal, how would it sound. (Leave out or invert preprocessing as well)
- Is Rprop better than Momentum as it does directly turn around if the gradient changes sign while Momentum only slows down? (Jumps over minima vs miss minima)
- What is the difference in pretraining with stacking autoencoders to stacking RBMs? (I know that autoencoders can be used for denoising, so stacked DAs should be better for noisy signals, but what about plain autoencoders vs RBM)
- Does a trained Hopfield net always have spurious state
- Bild mit zick zac
