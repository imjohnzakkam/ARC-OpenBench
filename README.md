# ARC-OpenBench

ARC-OpenBench is an open-source toolkit and benchmarking suite designed for the Abstraction and Reasoning Corpus (ARC) challenge. This repository provides a comprehensive framework for developing, training, and evaluating machine learning models on the ARC dataset. It aims to facilitate research and experimentation by offering a modular and extensible platform that integrates state-of-the-art models and utilities.

## Features

- **Model Registry**: Easily register and manage different models using a flexible registry system.
- **Configuration-Based Setup**: Define experiments and model configurations using simple YAML files.
- **Data Handling**: Efficient data loading and preprocessing tailored for ARC's unique JSON format.
- **Training and Evaluation**: Comprehensive scripts for training and validating models with customizable settings.
- **Modular Design**: Extensible architecture allowing seamless integration of new models and components.
- **Built-In Models**: Includes implementations of baseline models and state-of-the-art approaches like ST-MoE.
- **Community-Driven**: Encourages collaboration and contributions from the research community to advance ARC challenge solutions.

## Getting Started

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/ARC-OpenBench.git
   cd ARC-OpenBench
   ```

2. **Install Dependencies**:
   ```bash
   pip install -e .
   ```

4. **Run Training for Baseline Model**:
   ```bash
   python train.py --config Baseline.yaml
   ```

5. **Run Training for ST-MoE Model**:
   ```bash
   python train.py --config ST-MoE.yaml
   ```

## Directory Structure

```
ARC-OpenBench/
├── data
│   ├── train
│   └── val
├── solver
│   ├── losses
│   ├── metrics
│   ├── models
│   │   ├── baseline_model.py
│   │   └── st_moe.py
│   ├── ops
│   └── utils
├── configs
│   ├── Baseline.yaml
│   └── ST-MoE.yaml
├── scripts
├── train.py
├── test.py
├── README.md
├── setup.py
└── utils
    ├── config_loader.py
    └── registry.py
```

## Contributing

We welcome contributions from the community to improve ARC-OpenBench. If you have any suggestions, feature requests, or would like to contribute code, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License.
