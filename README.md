# Enhanced Siamese Network for One-Shot Image Recognition

This repository hosts the enhanced Siamese Neural Network for one-shot image recognition tasks. The model is based on the original work but includes significant improvements for better performance and generalization.

## Original Work
The original Siamese Network, as introduced in [this paper](https://paperswithcode.com/paper/siamese-neural-networks-for-one-shot-image), laid the foundation for one-shot image recognition tasks. It introduced the concept of allowing models to classify data points correctly after exposure to only a single example from each class during training.
The orginal code can be cloned from this [repository](https://github.com/sorenbouma/keras-oneshot/tree/master).

## Motive
- Humanizing the concept of machine learning
- Learn to classify and recognize things with a limited data
- Ability of a model to classify data points correctly after being exposed to only a single example from each class during training.

## Performance Comparison

We have improved the original Siamese Network by introducing various techniques such as data augmentation, dropout regularization, and attention mechanisms. The following tables and graphs highlight the comparative performance of the original and modified codes.

### Original vs. Modified Code Performance Table

| Epochs | Original Loss | Original Validation Accuracy (%) | Modified Loss | Modified Validation Accuracy (%) |
|--------|---------------|----------------------------------|---------------|----------------------------------|
| 1      | 4.521         | 7.2                              | 4.175         | 50.0                             |
| 5      | 4.40          | 16.8                             | 2.5693        | 66.5                             |
| 10     | 4.23          | 29.2                             | 1.338         | 71.2                             |
| 15     | 4.07          | 36.4                             | 0.979         | 70.1                             |


### Visual Comparison of Model Performance

The following visualizations show a clear difference in the training loss and validation accuracy between the original implementation and the modified implementation.

#### Original Implementation Graphs
![Screenshot 2024-04-19 121401](https://github.com/FawazSapa/Siamese_Network/assets/114939768/11570280-94ad-4d3f-a666-d644a72f7e8c)


#### Modified Implementation Graphs
![Screenshot 2024-04-19 121448](https://github.com/FawazSapa/Siamese_Network/assets/114939768/bb1c5b12-0fa5-4892-9f07-e5157d66d992)


## Enhancements

The model enhancements are detailed below:

- **Data Augmentation**: To aid the model in learning invariant features and to improve robustness against overfitting.
- **Dropout Regularization**: Implemented post MaxPooling layers to enforce robust feature learning.
- **Attention Mechanism**: Allows the network to focus on the most significant parts of the image.
- **Regularization Techniques**: L2 regularization was applied to control model complexity and prevent overfitting.

## Conclusion

The enhanced Siamese network showcases a substantial improvement over the original implementation. The introduction of data augmentation, dropout regularization, and attention mechanisms has not only improved the validation accuracy but also helped the model generalize better, evidenced by the reduced loss. These enhancements are essential for the model's application in scenarios where data is limited, making the Siamese network a more effective tool for one-shot learning tasks.

## Installation

Clone the repository and install the necessary dependencies:

```bash
git clone https://github.com/your-username/your-repository.git
cd your-repository
pip install -r requirements.txt
