# 🚀 DepGeist - The Smart Dependency Manager for Python

**DepGeist** is an intelligent dependency manager that scans your Python project, detects missing or unused dependencies, and suggests updates in seconds.

## 🎯 Features  
✅ **Scans Your Project** - Detects dependencies used in your code.  
✅ **Finds Missing Dependencies** - Alerts you about packages you forgot to install.  
✅ **Detects Unused Dependencies** - Cleans up your `requirements.txt`.  
✅ **Suggests Updates** - Recommends package updates based on PyPI versions.  
✅ **Works via CLI & Python API** - Use it in scripts or the terminal.  

---

## 📦 Installation  
You can install **DepGeist** via pip:

```sh
pip install depgeist
```

---

## 🚀 Quick Start  

### **CLI Usage**  
After installation, use `depgeist` in your terminal:  

```sh
depgeist scan        # Scan the project for dependencies  
depgeist check       # Check for missing/extra dependencies  
depgeist update      # Suggest updates for outdated dependencies  
```

---

### **Python API Usage**  
DepGeist can also be used programmatically:  

```python
import depgeist

# Scan the project for dependencies
dependencies = depgeist.scan_project(".")

# Check for missing and extra dependencies
missing, extra = depgeist.check_dependencies()

# Suggest updates for outdated dependencies
outdated = depgeist.suggest_updates()
```

---

## 📜 Example Output  

```sh
$ depgeist check
🔍 Scanning project...
✅ Found dependencies: requests, numpy, pandas
⚠️ Missing dependencies: requests
🗑️ Unused dependencies: pandas
```

```sh
$ depgeist update
📌 Checking for outdated dependencies...
🔄 numpy 1.21.0 → 1.25.2  (latest)
```

---

## 🤝 Contributing  
We welcome contributions! Fork the repo, make changes, and submit a PR.  

1. Clone the repo:  
   ```sh
   git clone https://github.com/ibrahims-main/DepGeist.git
   cd depgeist
   ```

2. Open a pull request! 🚀  

---

## ⚖️ License  
DepGeist is open-source and licensed under the [MIT License](LICENSE).  

---

## ⭐ Support the Project  
If you find **DepGeist** useful, please **star** the repo and share it with others! 🌟  