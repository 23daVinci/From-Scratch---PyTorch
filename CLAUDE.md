# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

A personal learning repo for implementing PyTorch exercises from scratch. Exercises are adapted from [TorchLeet](https://github.com/Exorust/TorchLeet) and live as Jupyter notebooks (the notebooks keep TorchLeet's Colab badge and problem statement as markdown cells at the top, followed by starter code with `#TODO` markers for the user to fill in).

## Layout

- `Basics/` — one notebook per exercise (currently `lin_regression.ipynb`). New exercises go in a notebook here, each self-contained: problem statement cell, imports, synthetic data + model + training loop, then an evaluation cell.
- `main.py` — uv-generated placeholder; not part of any exercise.
- `pyproject.toml` — uv-style project, Python `>=3.13` (`.python-version` is 3.13). `dependencies` is empty: torch is **not** declared, so it must be installed in the environment before running notebooks (e.g. `uv add torch`).

## Commands

There is no build, lint, or test setup. Exercises are run by executing notebook cells (Jupyter/VS Code/Colab). The TorchLeet check helper (`pip install torchleet`; `check("lin-regression", ...)`) is referenced in the notebooks but is not a project dependency.

## Notes

- Notebooks are works in progress and may contain deliberate gaps or bugs (e.g. `lin_regression.ipynb` currently uses `nn.parameter` instead of `nn.Parameter`, uses the global `X` instead of `x` in `forward`, and the final cell references `model.linear` which doesn't exist on the hand-rolled model). Don't "fix" these unprompted; the user is working through the exercises.
