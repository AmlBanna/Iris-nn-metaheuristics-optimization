# 🌼 Iris Neural Network Optimization with Metaheuristic Algorithms

This project explores the use of various **metaheuristic algorithms** (GA, GWO, ABC, PSO, Firefly, ACO, OBC-WOA) to optimize the hyperparameters of a **Neural Network** model trained on the **Iris dataset**.

## 🧠 Objective

To improve the classification accuracy of a neural network by automatically selecting the best:
- Learning rate (log-scale)
- Number of hidden layers
- Number of neurons per layer

## 🧪 Dataset

- **Dataset**: [Iris Dataset](https://scikit-learn.org/stable/auto_examples/datasets/plot_iris_dataset.html)
- **Features**: 4 numeric attributes (sepal/petal length/width)
- **Target**: 3 flower classes (setosa, versicolor, virginica)

## 🏗️ Model Architecture

- Input layer: 4 features
- Hidden layers: dynamic (based on optimization)
- Activation: ReLU
- Output layer: 3 classes with Softmax

## ⚙️ Optimization Algorithms Used

The following algorithms were used to tune the neural network:
- 🔬 Genetic Algorithm (GA)
- 🐺 Grey Wolf Optimizer (GWO)
- 🔥 Firefly Algorithm
- 🐜 Ant Colony Optimization (ACO)
- 🐝 Artificial Bee Colony (ABC)
- 🌪️ Particle Swarm Optimization (PSO)
- 🌀 Opposition-Based Chaotic Whale Optimization Algorithm (OBC-WOA)

Each algorithm tries to maximize classification **accuracy** by searching the best hyperparameters.

## 🧾 Output

The results of each optimizer (best parameters and accuracy) are saved in a Word file:  
📄 `optimization_results.docx`

## 🧰 Requirements

```bash
tensorflow
scikit-learn
deap
numpy
python-docx
```

Install via:
```bash
pip install -r requirements.txt
```

## 📈 Example Results (Excerpt)

| Algorithm   | Best Accuracy | Best Parameters                  |
|-------------|---------------|----------------------------------|
| GA          | 96.7%         | `[-3.01, 2, 35.3]`               |
| GWO         | 100%          | `[-3.06, 1.55, 39.2]`            |
| PSO         | 100%          | `[-2.49, 1, 28]`                 |
| Firefly     | 100%          | `[-1.89, 1.13, 8.06]`            |
| OBC-WOA     | 96%           | `[-1, 1, 23.67]`                 |


