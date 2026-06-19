## **MLP Digit Classifier: From Theory to Interactive Web App**

A complete implementation of a multilayer perceptron (MLP) neural network trained on MNIST, spanning from NumPy-only backpropagation to a gorgeous interactive web interface [with a lot of AI assistance, don't call me a vibe coder please :( ]

### **Backend: Pure Python Neural Network** 
- **3-layer MLP** with ReLU hidden activations and softmax output
- **From scratch**: forward pass, categorical cross-entropy loss, and backpropagation
- **60,000 training samples** (MNIST) with mini-batch gradient descent
- **Achieves >97% test accuracy** in 40 epochs
- Includes PyTorch gradient verification to validate correctness
- Weights exported as JSON for inference

### **Frontend: Interactive Drawing Canvas** 
- **Real-time digit prediction** as you draw on a 280×280 canvas
- **Animated background particle system** with smooth gradients
- **Pop animation** on prediction with particle burst at >80% confidence
- **Live confidence bars** showing probability distribution across all 10 digits
- **Reduced-motion support** for accessibility
- Minimal dependencies (vanilla JS + Canvas API)

### **Features**
- MNIST dataset auto-downloads on first run
- One-hot encoding, data normalization, shuffling
- Detailed epoch-by-epoch loss tracking and accuracy metrics
- Sample predictions grid (one per digit class)
- Trained weights can be deployed anywhere via JSON

### **Tech Stack**
- **Notebook**: NumPy, Matplotlib
- **Web**: Vanilla JavaScript, HTML5 Canvas, CSS3 animations
- **Optional**: PyTorch (gradient verification only)

### **Quick Start**
1. Run the Jupyter notebook to train the MLP (outputs `weights.json`)
2. Place `weights.json` next to index.html
3. Open index.html in a browser and start drawing digits
