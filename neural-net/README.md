# neural-net

A tiny scalar-valued autograd engine and neural network, built from scratch, then rebuilt in PyTorch for comparison.

Built following Andrej Karpathy's [micrograd lecture](https://karpathy.ai/zero-to-hero.html).

## What's here

| File | What it is |
|---|---|
| [`engine.py`](engine.py) | `Value`: a scalar that tracks how it was computed, with `.backward()` for automatic differentiation |
| [`nn.py`](nn.py) | `Neuron`, `Layer`, `MLP` built on top of `Value` |
| [`viz.py`](viz.py) | `draw_dot`: renders the computation graph with each node's data and gradient |
| [`demo.ipynb`](demo.ipynb) | Backprop through a single neuron, a PyTorch gradient check, and training an MLP |
| [`pytorch-makemoons-demo.ipynb`](pytorch-makemoons-demo.ipynb) | The same network rebuilt in PyTorch |
| [`backprop-notes.pdf`](backprop-notes.pdf) | My handwritten derivation of one full training step on a 2 → 2 → 1 network |
| [`lecture-notes.ipynb`](lecture-notes.ipynb) | Raw working notebook from following the lecture |
