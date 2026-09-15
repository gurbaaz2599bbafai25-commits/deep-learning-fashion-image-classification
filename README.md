# Deep Learning Fashion Image Classification

A beginner-friendly Deep Learning project that uses **TensorFlow/Keras** and the **Fashion MNIST** dataset to automatically classify fashion product images into 10 different categories.

The project demonstrates how Artificial Neural Networks can be applied to a real-world **e-commerce product categorization** problem.

## 📌 Project Overview

E-commerce companies receive thousands of product images that need to be categorized before products are listed on their websites. Manually categorizing every image can be time-consuming and repetitive.

This project demonstrates an AI-assisted approach where a Deep Learning model analyzes a product image and predicts its category.

### Business Problem

**Manual Process:**

Product Image → Employee → Manual Category Selection → Product Listing

### AI-Assisted Process

Product Image → Deep Learning Model → Predicted Category → Human Review → Product Listing

---

## 🎯 Objectives

* Understand how images can be used as input for Deep Learning.
* Build a simple Artificial Neural Network.
* Understand input, hidden, and output layers.
* Train a model using fashion product images.
* Evaluate model accuracy.
* Predict categories for unseen images.
* Understand the business applications and limitations of image classification.

---

## 🗂️ Dataset

The project uses the **Fashion MNIST** dataset provided through TensorFlow/Keras.

The dataset contains grayscale images of fashion products belonging to 10 categories:

| Label | Category    |
| ----: | ----------- |
|     0 | T-shirt/Top |
|     1 | Trouser     |
|     2 | Pullover    |
|     3 | Dress       |
|     4 | Coat        |
|     5 | Sandal      |
|     6 | Shirt       |
|     7 | Sneaker     |
|     8 | Bag         |
|     9 | Ankle Boot  |

Each image has a resolution of **28 × 28 pixels**.

---

## 🧠 Model Architecture

The project uses a simple Artificial Neural Network:

```text
Input Image
     ↓
Flatten Layer
     ↓
Dense Layer (64 neurons)
     ↓
ReLU Activation
     ↓
Output Layer (10 neurons)
     ↓
Softmax
     ↓
Predicted Fashion Category
```

### Model Components

* **Flatten:** Converts the 28 × 28 image into a one-dimensional format.
* **Dense(64):** Hidden layer containing 64 neurons.
* **ReLU:** Activation function used in the hidden layer.
* **Dense(10):** Output layer with 10 neurons, one for each category.
* **Softmax:** Produces probabilities for the 10 possible categories.

---

## ⚙️ Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib
* Fashion MNIST
* Google Colab / Jupyter Notebook

---

## 🔄 Project Workflow

1. Import required Python libraries.
2. Load the Fashion MNIST dataset.
3. Define the product categories.
4. Visualize sample images.
5. Normalize pixel values from 0–255 to 0–1.
6. Create the Artificial Neural Network.
7. Compile the model using the Adam optimizer.
8. Train the model for 3 epochs.
9. Evaluate the model on unseen test data.
10. Generate predictions for new images.
11. Compare predicted and actual categories.
12. Interpret the results from a business perspective.

---

## 📊 Model Training

The model is trained using:

* **Optimizer:** Adam
* **Loss Function:** Sparse Categorical Crossentropy
* **Metric:** Accuracy
* **Epochs:** 3
* **Validation Split:** 10%

The exact test accuracy can vary slightly between runs.

After running the notebook, the test accuracy is displayed in the output.

---

## 💼 Business Application

This model can assist an e-commerce company with automatic product categorization.

### Potential Benefits

* Faster product listing
* Reduced repetitive manual work
* More consistent product categorization
* Improved product search and filtering
* Ability to process a large number of product images

### Human Oversight

The model should not necessarily replace employees completely.

A practical implementation could use:

**AI Prediction → Human Review → Final Product Category**

Human review can be particularly useful when the model has low confidence or when an incorrect classification could negatively affect customers.

---

## ⚠️ Limitations

* The model is trained on a relatively simple dataset.
* Fashion MNIST images are small grayscale images.
* Real-world product images can be much more complex.
* Similar-looking products may be incorrectly classified.
* Accuracy alone does not determine whether an AI system is ready for business deployment.
* Human oversight may still be required.

---

## 📁 Repository Structure

```text
deep-learning-fashion-image-classification/
│
├── Deep_Learning_Fashion_Classification_Name.ipynb
├── README.md
└── screenshots/
    └── prediction.png
```

---

## 🚀 How to Run

### Option 1: Google Colab

1. Open the `.ipynb` notebook in Google Colab.
2. Run the cells sequentially.
3. The Fashion MNIST dataset will be downloaded automatically.
4. Train the model.
5. Check the test accuracy.
6. Try different image numbers to test predictions.

### Option 2: Jupyter Notebook

Install the required libraries:

```bash
pip install tensorflow numpy matplotlib
```

Then open the notebook and run the cells.

---

## 🧪 Example Prediction

The notebook allows the model to predict the category of an unseen fashion image.

Example:

```text
Predicted Product: Sneaker
Actual Product: Sneaker
```

The notebook also allows different test images to be selected by changing the `image_number` variable.

---

## 📚 Learning Outcomes

Through this project, the following concepts are demonstrated:

* Image classification
* Artificial Neural Networks
* Input, hidden and output layers
* Feature learning
* Activation functions
* Model training
* Model testing
* Accuracy evaluation
* Prediction on unseen data
* AI applications in business
* Human-AI collaboration

---

## 👨‍💻 Project Type

**Academic Project | BBA AI/ML | Deep Learning Practical**

This project was created to demonstrate the practical application of Deep Learning to an e-commerce business problem.

---

## 📌 Conclusion

The project demonstrates how a simple Artificial Neural Network can learn patterns from fashion images and classify them into predefined product categories.

While the model provides an effective demonstration of image classification, real-world deployment would require more advanced models, larger and more diverse datasets, extensive testing, and appropriate human oversight.

> **Key Takeaway:** AI can automate repetitive business processes, but organizations should consider accuracy, risk, data quality, and human oversight before deploying an AI system.
