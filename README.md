
# MNIST Classification: SNN vs CNN Comparative Study

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-ee4c2c.svg)](https://pytorch.org/)

## Overview

Comparative implementation of **Spiking Neural Networks (SNNs)** vs traditional **CNNs** for MNIST digit classification with energy efficiency analysis.

### Key Results
- **SNN Accuracy**: 98.27%
- **CNN Accuracy**: 98.90%  
- **Energy Efficiency**: 18.7x reduction with SNNs
- **Accuracy Gap**: Only 0.63%

## Quick Start
```bash
pip install torch torchvision snntorch matplotlib seaborn scikit-learn
python mnist_snn_comparison.py
```

## Results Summary

| Model | Accuracy | Energy (µJ) | Operations |
|-------|----------|-------------|------------|
| SNN   | 98.27%   | 1.68        | 2.1e7      |
| CNN   | 98.90%   | 31.45       | 8.5e8      |

**Trade-off**: 0.63% accuracy reduction for 18.7x energy savings

## Architecture

### SNN
- Leaky Integrate-and-Fire neurons
- 25 time steps with rate coding
- Surrogate gradient training
- Event-driven processing

### CNN  
- Standard ConvNet baseline
- Same layer structure for fair comparison
- Dense operations

## Applications
- Battery-powered edge devices
- IoT sensors with power constraints
- Portable medical diagnostics
- Green AI initiatives

## Files
- `MNIST_SNN_Comparison.ipynb` - Full implementation
- `results/` - Figures and metrics
- `requirements.txt` - Dependencies

## Citation
```bibtex
@misc{yourusername2025mnist,
  title={MNIST SNN vs CNN: Energy Efficiency Study},
  author={Your Name},
  year={2025},
  url={https://github.com/yourusername/mnist-snn-energy-efficiency}
}
```

## License
MIT
