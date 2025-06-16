# Neural Network from Scratch - Cat Classifier 🐱

Welcome to my small project where I built a **neural network from scratch** in NumPy to classify images (like the cute one below 🐾). This isn't just another model using a fancy library; this is the raw math and logic behind how deep learning works.

![Cat Classifier](./Cat%20Photo.png)

---

## 🚀 What I Built

I implemented:

### ✅ Two-Layer Neural Network
Structure: `LINEAR -> RELU -> LINEAR -> SIGMOID`  
This is the basic neural network to understand how forward and backward propagation work.

### ✅ L-Layer Deep Neural Network
Structure: `[LINEAR -> RELU] x (L-1) -> LINEAR -> SIGMOID`  
This generalizes the above model for deeper networks. It's flexible for any number of layers.

---

## 🛠️ Functions Implemented

Here are the major building blocks I coded:

- `initialize_parameters()` and `initialize_parameters_deep()` – to randomly initialize weights and biases
- `linear_activation_forward()` – to perform linear + activation in one go
- `compute_cost()` – computes binary cross-entropy loss
- `linear_activation_backward()` – applies chain rule for backpropagation
- `update_parameters()` – gradient descent update rule
- `two_layer_model()` – the full 2-layer model using the above blocks
- `L_layer_model()` – the general deep model for any layer architecture

---

## 📈 Training

Each model was trained using **gradient descent**. The cost is printed every 100 iterations to show progress. There's also a helper to **plot the cost curve** so we can visualize convergence.

```python
plot_costs(costs)
