# 🐍 Marketing Analytics Lab Setup (VS Code + Python + Jupyter)

This guide helps you set up your development environment for running this project using Visual Studio Code, Python virtual environments, and Jupyter notebooks.

---

## ✅ Prerequisites

- Windows / Mac / Linux system
- Admin rights to install software

---

## 🚀 Setup Steps

### 1️⃣ Install Visual Studio Code

- Download and install **VS Code**:  
  [https://code.visualstudio.com/](https://code.visualstudio.com/)

---

### 2️⃣ Install Python

- Download and install **Python 3.9 or higher**:  
  [https://www.python.org/downloads/](https://www.python.org/downloads/)
  
- During installation, ensure you check:
  - ✅ **Add Python to PATH**

---

### 3️⃣ Install VS Code Extensions

In VS Code, open the **Extensions** view (`Ctrl+Shift+X`) and install:

- **Python** (by Microsoft)  
- **Jupyter** (by Microsoft)

---

### 4️⃣ Create and Activate Virtual Environment

- Open your project folder in VS Code.
- Open a terminal (`Ctrl+``).

Create a virtual environment:
```bash
python -m venv venv
```

Activate the environment:

- On **Windows**:
```bash
venv\Scripts\activate
```

- On **Mac/Linux**:
```bash
source venv/bin/activate
```

---

### 5️⃣ Select Python Interpreter (venv Kernel)

- Press `Ctrl+Shift+P` → type and select **Python: Select Interpreter**
- Choose the interpreter from your local `./venv` folder

---

### 6️⃣ Update pip, setuptools, wheel

```bash
python -m pip install --upgrade pip setuptools wheel
```

---

### 7️⃣ Install Project Requirements

```bash
pip install -r requirements.txt
```

---

## ✅ You’re Ready!

You can now:
- Run Python scripts (`.py`)
- Launch and edit **Jupyter notebooks (`*.ipynb`)** directly in VS Code

---

## 🛠️ Troubleshooting Tips

### Python Not Found
- Ensure Python is added to PATH during installation.
- Verify by running:
```bash
python --version
```

---

### Virtual Environment Not Showing in VS Code
- Manually select the interpreter:
    - `Ctrl+Shift+P` → **Python: Select Interpreter** → pick `./venv`

---

### Jupyter Kernel Not Found
- Activate your virtual environment and install Jupyter:
```bash
pip install jupyter
```

---

### Package Installation Failures
- Upgrade pip, setuptools and wheel:
```bash
python -m pip install --upgrade pip setuptools wheel
```

- If building wheels fails on Windows, install **Visual C++ Build Tools**:  
  [https://visualstudio.microsoft.com/visual-cpp-build-tools/](https://visualstudio.microsoft.com/visual-cpp-build-tools/)

---

### VS Code Not Detecting venv
- Restart VS Code after creating the virtual environment.
- Ensure `python.defaultInterpreterPath` is set in `.vscode/settings.json`:
```json
{
    "python.defaultInterpreterPath": "venv\\Scripts\\python.exe"
}
```

---
