# From-Scratch---PyTorch

A collection of neural network architectures implemented from scratch in PyTorch. The goal is to understand how each model works by building it piece by piece instead of relying on pre-built implementations.

## Repository Structure

```
.
├── Basics/                  # Foundational models, one notebook per exercise
│   ├── lin_regression.ipynb
│   ├── custom_dataset.ipynb
│   └── custom_activation.ipynb
├── main.py
├── pyproject.toml
└── README.md
```

Each architecture lives in its own notebook. A notebook states the problem, builds the model, trains it, and evaluates it.

## Current Implementations

| Architecture | Location | Status |
|---|---|---|
| Linear Regression | `Basics/lin_regression.ipynb` | In progress |
| Custom Dataset and DataLoader (CSV) | `Basics/custom_dataset.ipynb` | Done |
| Custom Activation Function (`tanh(x) + x`) | `Basics/custom_activation.ipynb` | Done |

More architectures will be added over time.

## Getting Started

### Requirements

- Python 3.13 or later
- [PyTorch](https://pytorch.org/get-started/locally/)
- pandas (used by the custom dataset notebook)
- Jupyter, or any editor that can run notebooks (VS Code, Colab)

### Setup

```bash
git clone <repo-url>
cd From-Scratch---PyTorch
uv add torch pandas jupyter   # or: pip install torch pandas jupyter
jupyter notebook
```

Then open a notebook in `Basics/` and run the cells in order.

## Acknowledgements

Some exercises are adapted from [TorchLeet](https://github.com/Exorust/TorchLeet).

## License

See [LICENSE](LICENSE).
