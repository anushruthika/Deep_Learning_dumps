1. perceptron? fundamental building block, gets input feature associated with weights , learn from weights and baises . Then activation function for non-linearity. Back-propogation(optimizers)
2.ANN working: foward propogation
3. Weights: Determine the importance of each input feature.
4. Bias: An additional learnable parameter that shifts the decision boundary.
5. activation function
6. sigmoid: vanishing gradient descent, non-centred around zero : 1/1+e^-z
7. Tanh: vanishing gradient descent, centered around Zero: (e^z - e^(-z)) / (e^z + e^(-z))
8. Backward Propagation chain rule of differntiation:
    **Take a single neuron:**
    z = wx + b
    a = σ(z)
    
    **Using Mean Squared Error:**
    L = ½(a − y)²
    
    **Derive the gradient using Chain Rule:**
    ∂L/∂w = (∂L/∂a) × (∂a/∂z) × (∂z/∂w)
    
    **Substituting:**
    ∂L/∂w = (a − y) × a(1 − a) × x
    similarly find for dl/db
  
9.Loss function: regression: MSE,MAE,huber loss, Classification: binary entropy , cross entropy, kl divergance, hinge loss
10. how to prevent over fitting? early stopping(where training is stopped once the model’s performance on a validation set stops improving), drop out(drop neurons), batch normalization(normalize the inputs of each layer so that they have a consistent distribution during training).
11. 

   
