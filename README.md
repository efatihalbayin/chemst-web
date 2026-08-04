# 🧪 ChemST - Smart Chemical Solution & PubChem Assistant

![Python Version](https://img.shields.io/badge/python-3.8%2B-blue.svg)
![Flutter](https://img.shields.io/badge/Flutter-3.x-02569B?logo=flutter)
![FastAPI](https://img.shields.io/badge/FastAPI-0.100%2B-009688?logo=fastapi)
![License](https://img.shields.io/badge/license-MIT-green.svg)

**ChemST**, laboratuvar ortamında kimyagerler, araştırmacılar ve öğrenciler için çözelti hazırlama, seyreltme hesaplamaları ve PubChem veritabanı sorgularını saniyelere indiren modern, açık kaynaklı bir kimya asistanıdır.

---

## 🚀 Canlı Demo (Live Demo)

Web uygulamasını hemen denemek için:
👉 **[ChemST Web Application Live](https://efatihalbayin.github.io/chemst-web/)**

---

## ✨ Öne Çıkan Özellikler (Key Features)

- 🔍 **PubChem Live Search:** Molekül adıyla saniyeler içinde IUPAC adı, PubChem CID ve Molekül Ağırlığı ($MW$) sorgulama.
- ⚖️ **Molar Çözelti Hesaplayıcı:** Hedef Molarite ($M$), Hacim ($mL$), Saflık (%) ve Hidrat Suyu ($H_2O$) katsayılarını dikkate alarak hassas kütle reçetesi oluşturma.
- 💧 **Seyreltme Matrisi ($C_1V_1 = C_2V_2$):** Stok çözeltiden çekilecek hacmi ve eklenmesi gereken çözücü miktarını anında hesaplama.
- 🎨 **Modern & Dark UI:** Laboratuvar ortamında gözü yormayan şık ve responsive koyu tema arayüzü.

---

## 🏗️ Sistem Mimarisi (System Architecture)

Proje, 3 katmanlı modüler bir yazılım mimarisi üzerine inşa edilmiştir:

```text
[ 🌐 Flutter Web / Mobile Frontend ]
                 │
                 ▼  (REST API - JSON)
[ ⚡ FastAPI Backend Engine (Render) ]
                 │
                 ▼  (Core Logic)
[ 🧪 chemst Core Python Package (PyPI) ]
