# AI651 Assignment 2: Deep Learning for Space, Time and Graphs

Fall 2026, LUMS. Author: YOUR NAME (ROLL NO)

## Layout
- `q1/`: River forecasting proposal (LaTeX sources, diagrams).
- `q2/q2_experiments.ipynb`: Moving MNIST experiments (ConvLSTM, symmetry and speed tests).
- `q2/predictions/`: predictions written BEFORE the experiments they refer to (Q2.5, Q2.11). Never edited after commit.
- `q2/results/`: tables, figures, GIFs.

## Running Q2
1. `pip install torch torchvision opencv-python matplotlib numpy`
2. Open `q2/q2_experiments.ipynb`.
3. Debug first with `SMOKE = True` (fake data, 1 epoch). For the real run set `SMOKE = False` and restart the kernel.
4. Data: `torchvision.datasets.MovingMNIST(split=None)` is downloaded to `./data` (git-ignored).

## Reproducibility
- Split by video index: 0-7999 train, 8000-8999 validation, 9000-9999 test.
- Every learned model is trained with seeds 0 and 1.
- Hardware and timings are printed by the notebook.

## Generative AI use
See `ai_usage.md` (prompt, output, edits).
