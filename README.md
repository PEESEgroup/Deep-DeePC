# Deep-DeePC
We propose a data-enabled predictive control framework using a deep neural network (Deep DeePC) for greenhouse climate control systems. This integration enables efficient approximation of the complex mappings required for predictive control, significantly reducing the computational burden during online implementation. To handle climate and actuator constraints effectively, we also implement a differentiable QP layer as end-to-end learning architecture. For a numerical case study using the outdoor climate data in Colombus, OH, we compared the proposed Deep DeePC framework with a nonlinear model predictive control (NMPC) baselimne and standard DeePC. The results demonstrate effective climate management for lettuce and underscore the approach’s potential scalability and generalizability to other greenhouse crops and operating conditions.
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
