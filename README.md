<p align="center">
  <img src="logo.png" alt="ChemST Logo" width="200"/>
</p>

# ChemST - Smart Chemical Solution & PubChem Assistant

![Python Version](https://img.shields.io/badge/python-3.8%2B-blue.svg)
![Flutter](https://img.shields.io/badge/Flutter-3.x-02569B?logo=flutter)
![FastAPI](https://img.shields.io/badge/FastAPI-0.100%2B-009688?logo=fastapi)
![License](https://img.shields.io/badge/license-MIT-green.svg)
---

## Live Demo

Try the live web application:
[ChemST Web Application](https://efatihalbayin.github.io/chemst-web/)

---

## Key Features

- **PubChem Live Search:** Query IUPAC names, PubChem CID, and Molecular Weight ($MW$) by compound name.
- **Molar Solution Calculator:** Generate precise mass recipes considering target Molarity ($M$), Volume ($mL$), Purity (%), and Hydration Water ($H_2O$) coefficients.
- **Dilution Matrix ($C_1V_1 = C_2V_2$):** Instant calculation of required stock volume and additional solvent volume.
- **Modern Dark UI:** Clean, responsive dark-themed interface optimized for laboratory environments.

---

## System Architecture

The project is built on a 3-tier modular software architecture:

```text
[ Flutter Web / Mobile Frontend ]
                 │
                 ▼  (REST API - JSON)
[ FastAPI Backend Engine (Render) ]
                 │
                 ▼  (Core Logic)
[ chemst Core Python Package (PyPI) ]
```

1. **Core Package:** The `chemst` Python library published on PyPI.
2. **Backend Service:** A FastAPI microservice running 24/7 on Render.
3. **Frontend:** Single-codebase Flutter Web / PWA client application.

---

## Local Development

### 1. Install Python Package (`chemst`)

```bash
pip install chemst

```

### 2. Run API Service Locally

```bash
git clone [https://github.com/efatihalbayin/chemst-api.git](https://github.com/efatihalbayin/chemst-api.git)
cd chemst-api
pip install -r requirements.txt
uvicorn main:app --reload

```

### 3. Run Flutter Web Frontend

```bash
git clone [https://github.com/efatihalbayin/chemst-web.git](https://github.com/efatihalbayin/chemst-web.git)
cd chemst-web
flutter pub get
flutter run -d chrome

```

---

## License

This project is licensed under the [MIT License](https://www.google.com/search?q=LICENSE). Feel free to fork, modify, and contribute.

---

Developed for Chemists & Researchers.

```

```
