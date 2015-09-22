
ANN vs BNN
----------

Perceptron
----------
- X1 and X2 are linear separable <=> exits separating hyperplan <=> convex hulls of X1 and X2 are disjoint
- Perceptron can only learn linear separable things
- \hat w^T x > 0 \forall x \in X_1 (t_x = 1)
  \hat w^T x \leq 0 \forall x \in X_2 (t_x = 0)
- Inverted data trick: negate input vectors for X_2 => new goal: find \hat w^T x > x 


Support Vector Machines
----------------------
- use kernels to transform data into higher dimensional space where it is linear separable


Generalization
--------------
for linear systemo: E_test = E_train + 2 \sigma^2 \frac{|\theta|}{n} mit \sigma = effective varianz of the noise

Reduzierung der Komplexität des NN durch:
- Weight decay
- Weight elimination (ähnlich L2 norm \gamme \sum_{i,j} \frac{w_{ij}^2}{1+w_{ij}^2})
- Optimial Brain Damage (simple: delete smallest weights, better delete weight that have lowest impact on error, calculate \frac{\partial E}{\partial w_{ij}^2})
- Optimial Brain Surgeon

Schrittweises Vergrößern eines zu kleinen Netzes durch
- Cascade Correlation (schrittweises hinzufügen von neuen Verbindungen)
- Meiosis Netzwerke (aufspalten eines neurons anhand von mean and varinz der Gewichte => zusätzliche Parameter)
- Automativ Structure Optimization


Recurrent Neural Networks
-------------------------
- Elman Networks vs Jordan Network
- Training with Backpropagation through time => unfold to FFNN with shared weights
- weight update dates are summed or averaged
- RNNs only use past context, some application (as speech) benefit from future context
	- => combine results from forword RNN with backword RNN
	- => stacked input context
	- => bi-directional RNN
	- => delayed outputs
- Vanishing Gradient
