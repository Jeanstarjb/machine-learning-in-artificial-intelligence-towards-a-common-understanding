# Machine Learning in Artificial Intelligence: Towards a Common Understanding

## Overview

This repository contains a Python implementation of the conceptual framework outlined in the research paper [Machine Learning in Artificial Intelligence: Towards a Common Understanding](https://arxiv.org/pdf/2004.04686v1) by Niklas Kühl, Marc Goutier, Robin Hirt, and Gerhard Satzger. The goal of the paper is to clarify the often overlapping and ambiguous use of the terms "machine learning" (ML) and "artificial intelligence" (AI). It provides a conceptual framework to better define the role of ML in achieving AI, with the aim of fostering clarity and encouraging interdisciplinary discussions.

This repository translates the theoretical concepts presented in the paper into a practical implementation using Python and PyTorch, enabling practitioners and researchers to explore and experiment with the ideas presented.

---

## Core Concept

The paper emphasizes the distinction and relationship between AI and ML:
- **Artificial Intelligence (AI):** The broader goal of creating intelligent agents capable of performing tasks that typically require human intelligence, such as reasoning, problem-solving, and decision-making.
- **Machine Learning (ML):** A subset of AI focused on designing algorithms and models that allow systems to learn patterns and make predictions or decisions based on data.

The authors propose a framework where ML serves as a critical enabler for building intelligent agents. By incorporating learning capabilities into agents, ML facilitates their ability to adapt to dynamic environments and solve complex problems.

---

## Repository Contents

This repository provides a Python implementation to illustrate the integration of ML within an AI framework. The code is structured to reflect the conceptual components discussed in the paper.

### Features
1. **Agent Framework:** A modular design for building intelligent agents that can incorporate learning capabilities.
2. **Reinforcement Learning (RL) Example:** Demonstrates how ML (specifically, RL) can be used to enable agents to make decisions in dynamic environments.
3. **Supervised Learning Integration:** A simple example of using supervised learning for classification tasks within an AI agent.
4. **Environment Interaction:** Simulations of agents interacting with environments to illustrate learning and adaptation.

---

## Getting Started

### Prerequisites
- Python 3.8 or higher
- PyTorch 2.0 or higher
- Additional dependencies listed in `requirements.txt`

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/ml-in-ai-framework.git
   cd ml-in-ai-framework
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Repository Structure

```
ml-in-ai-framework/
│
├── agents/
│   ├── base_agent.py          # Abstract base class for intelligent agents
│   ├── supervised_agent.py    # Agent using supervised learning
│   └── rl_agent.py            # Agent using reinforcement learning
│
├── environments/
│   ├── simple_env.py          # Example environment for agent interaction
│   └── __init__.py
│
├── models/
│   ├── ml_models.py           # Machine learning models (supervised and RL)
│   └── __init__.py
│
├── experiments/
│   ├── supervised_example.py  # Demonstration of supervised learning
│   ├── rl_example.py          # Demonstration of reinforcement learning
│   └── __init__.py
│
├── utils/
│   ├── plot_utils.py          # Utility functions for plotting results
│   └── __init__.py
│
├── requirements.txt           # List of dependencies
└── README.md                  # Project documentation
```

---

## How to Use

### 1. Supervised Learning Example
Run the supervised learning demonstration to see how an agent can perform classification tasks:
```bash
python experiments/supervised_example.py
```

Expected output:
- The agent trains on a dataset and evaluates its accuracy on a test set.
- Plots showing loss reduction and accuracy improvement over epochs.

### 2. Reinforcement Learning Example
Run the reinforcement learning demonstration to see how an agent learns to navigate a simple environment:
```bash
python experiments/rl_example.py
```

Expected output:
- The agent interacts with the environment and improves its policy over time.
- Visualization of the agent's performance and reward trends.

---

## Key Components

### 1. **Agents**
The `agents` module implements intelligent agents that can integrate various ML approaches:
- **BaseAgent:** Provides a common interface for all agents.
- **SupervisedAgent:** Implements agents using supervised learning techniques.
- **RLAgent:** Implements agents using reinforcement learning.

### 2. **Environments**
The `environments` module provides customizable environments for testing and training agents. These environments simulate tasks that agents must learn to solve.

### 3. **Models**
The `models` module defines the machine learning models used by the agents, including neural networks for supervised learning and RL-specific architectures.

### 4. **Experiments**
The `experiments` folder contains scripts to run specific examples, demonstrating how agents can utilize ML to perform tasks.

---

## Contributing

Contributions are welcome! If you'd like to enhance the framework, fix bugs, or add new features, please open an issue or submit a pull request. For major changes, consider discussing them in an issue first.

---

## References

- [Machine Learning in Artificial Intelligence: Towards a Common Understanding](https://arxiv.org/pdf/2004.04686v1) by Niklas Kühl, Marc Goutier, Robin Hirt, and Gerhard Satzger.
- [PyTorch Documentation](https://pytorch.org/docs/)

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.