# Group Project Setup Guide

## Project Content
- Gymnasium v1.2.2
- Part1 Sample Code
- Part2 Sample Code
- Part3 Sample Code
  
## Installation

```bash
# 1. Create a virtual environment
python -m venv .venv

# 2. Activate the virtual environment
source .venv/bin/activate

# 3. Navigate to the Gymnasium directory
cd group_project/Gymnasium

# 4. Install Gymnasium in editable mode
pip install -e .

# 5. Install additional dependencies
pip install "gymnasium[classic_control]"
pip install matplotlib
```

---

## ✅ Verification

Run the following command to verify that the installation is successful:

```bash
% pip list
```

Sample Output from MacOS:

```
Package              Version Editable project location
-------------------- ------- --------------------------------------------
cloudpickle          3.1.2
Farama-Notifications 0.0.4
gymnasium            1.2.2   ./group_project/Gymnasium
numpy                2.3.5
pip                  24.3.1
typing_extensions    4.15.0
```

If your output matches the above (or is similar), your environment is correctly configured.

---

## 🚀 Running the Project

### **Part 1: Mountain Car**
Train and test the reinforcement learning agent:

```bash
# Train the agent
python mountain_car.py --train --episodes 5000

# Render and visualize performance
python mountain_car.py --render --episodes 10
```

### **Part 2: Frozen Lake**
Run the Frozen Lake environment:

```bash
python frozen_lake.py
```

### **Part 3: OOP Project Environment**
Execute the custom OOP environment:

```bash
python oop_project_env.py
```

**Tip:**  
If you’re on Windows, replace  
```bash
source .venv/bin/activate
```  
with  
```bash
.venv\Scripts\activate
```
