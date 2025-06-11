# Deep-DeePC

Deep-DeePC is a data-enabled predictive control framework that leverages deep neural networks for real‐time greenhouse climate management. By learning the complex mapping from past measurements to future control actions, Deep-DeePC dramatically reduces the online computational load of traditional MPC schemes. To enforce physical and actuator constraints, we embed a differentiable quadratic programming (QP) layer directly into the end-to-end learning architecture.

In a numerical case study using outdoor climate data from Columbus, OH, we benchmark Deep-DeePC against a nonlinear MPC (NMPC) baseline and the standard DeePC algorithm. Our results on lettuce cultivation demonstrate superior climate regulation and highlight the approach’s scalability to other greenhouse crops and operating scenarios.

---

## Repository Structure

Deep-DeePC/
├── deep_deepc/ # Core implementation of the Deep-DeePC algorithm
│ ├── controller.py # Main controller class
│ ├── models.py # Neural network architectures
│ └── utils.py # Data loading & preprocessing
├── examples/ # Example scripts & notebooks
├── data/ # Sample climate datasets
├── tests/ # Unit tests
├── requirements.txt # Exact package versions
└── README.md # Project overview


---
## Codes
This folder contains the Python scripts used in the study. Details of each file or folder is provided below:

---
## Requirements
This project is designed for **Python 3.9** and depends on the core scientific and optimization libraries:
- PyTorch  
- NumPy  
- CVXPY  
- CVXPYlayers  
- SciPy  
- Matplotlib

All exact, tested versions are pinned in `requirements.txt`. To install them, simply run:

```bash
pip install -r requirements.txt
```

---

## Citation
Please use the following citation when using the data, methods or results of this work:

Kim, J., You, F. Energy-Efficient, Crop-Aware Intelligent Control for Smart Greenhouse with Deep DeePC Framework. Submitted to Applied Energy.
