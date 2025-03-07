### Steps to Build Quantum KNN

1. **Data Preparation**:
   - Collect and preprocess your dataset.
   - Normalize or standardize the data if necessary.

2. **Encoding Classical Data**:
   - Use a suitable encoding method (e.g., amplitude encoding, basis state encoding) to convert classical data into quantum states.

3. **Quantum Distance Measurement**:
   - Implement a quantum circuit that calculates the distance (e.g., Euclidean distance) between quantum states.

4. **Finding Neighbors**:
   - For each test instance, use the quantum circuit to find the `k` nearest neighbors from the training set.

5. **Voting Mechanism**:
   - Implement a voting mechanism to determine the class of the test instance based on the classes of the nearest neighbors.

6. **Prediction**:
   - Classify the test instance based on the majority vote from the neighbors.
  

### Steps to Build Quantum SVM

1. **Data Preparation**:
   - Collect and preprocess your dataset.
   - Convert categorical labels into numerical format (e.g., one-hot encoding).

2. **Quantum Feature Map**:
   - Design a quantum circuit that serves as a feature map to transform classical data into quantum states.

3. **Training the QSVM**:
   - Initialize weights for the hyperplane.
   - Use a quantum circuit to calculate the quantum features for each training instance.
   - Implement an optimization loop to adjust the weights based on classification errors.

4. **Prediction**:
   - For each test instance, calculate quantum features using the feature map.
   - Use the trained weights to determine the class of the test instance.


### Steps to Build Quantum NeuralNetworks 

the key difference i've met here was that we replace the nodes layers in the classical neural networks by the quantum gates (for basic cases we used a rotation) that work exactly like the nodes means the futur extraction 

1. **Circuit Building** : 
   - For the input layers we used BasisState for data transformation to quantum state 
   - Choosing the right gates (experementin with different gates)
   - Adding CNOT (for entanglement if needed)
   - simulate the backpropagation iterations (loss calculation >> weights update using gradient >> forward propagation for next row)