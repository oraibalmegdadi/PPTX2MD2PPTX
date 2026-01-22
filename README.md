# PPTX2MD2PPTX
# PPTX hookup ↔ Markdown Pipeline (Ubuntu)

This project provides a **round-trip conversion pipeline**:

**PowerPoint (.pptx) → Markdown (.md) → PowerPoint (.pptx)**

It preserves:
- Text content and formatting
- Absolute positioning (EMUs)
- Font styles and colors
- Images and hyperlinks
- Speaker notes
- Structured layout metadata

> ⚠️ Themes, slide masters, and animations are intentionally **not reconstructed automatically**  
> (they can be reapplied manually or via predefined layouts).

---

## 📦 Requirements (Ubuntu)

- Ubuntu 20.04+  
- Python **3.10+**
- `python3-venv`
- `pip`

Install system dependencies:

```bash
sudo apt update
sudo apt install -y python3-venv python3-pip
```

## 📁 Recommended Project Structure

pptx_md_pipeline/
├── pptx2md.py          # PPTX → Markdown
├── md2pptx.py          # Markdown → PPTX
├── config.json         # Styling / semantics config
├── sample/             # Extracted images
└── README.md


## 🧪 Virtual Environment Setup (Ubuntu)

Create a Python virtual environment:

```bash
python3 -m venv md2pptx

Activate the environment:

```bash
 md2pptx/bin/activate

#📦 Install Python Dependencies
```bash

pip install --upgrade pip
pip install python-pptx

