# 🖼️ Covex Texture Converter  
### PNG → DDS Converter for FiveM / GTA V  
**By Covex Studios**

Covex Texture Converter is a fast, modern, drag-and-drop tool for converting **PNG textures into DDS** formats commonly used in **FiveM**, **GTA V**, and other DirectX-based engines.

It uses **texconv.exe** (Microsoft DirectXTex) behind the scenes, wrapped in a clean, dark/light UI built with PySide6.

---

## 🚀 Features

- ✔ **Drag & drop PNG files or folders**  
- ✔ **Batch conversion** (hundreds at once)  
- ✔ **BC1 / BC3 / BC7 format support**  
- ✔ **FiveM preset** (BC3 + full mips)  
- ✔ **Dark / Light theme toggle**  
- ✔ **Real-time progress bar**  
- ✔ **Modern UI / Tailwind-like design**  
- ✔ **No flashing CMD windows**  
- ✔ **Icon fully embedded inside the EXE**  
- ✔ **Portable — no installation required**

---

## 📦 Folder Structure

Your release folder should look like:

CovexTextureConverter/
├─ CovexTextureConverter.exe    ← your app
├─ texconv.exe                  ← required for conversion
├─ pngs/                        ← place PNGs here
└─ output/                      ← converted DDS files appear here

> ⚠ IMPORTANT:  
> Do NOT remove `texconv.exe` — the converter cannot run without it.

---

## 🧑‍💻 How to Use

### 1. Drop PNGs
Drag & drop PNG files or entire folders onto the app window.  
They will be copied automatically into the `pngs/` folder.

### 2. Choose the output format
- BC1_UNORM — best for textures without alpha  
- BC3_UNORM — best for FiveM / GTA (supports alpha)  
- BC7_UNORM — modern high-quality compression  

### 3. Use the FiveM preset (recommended)
Click “For FiveM preset” → sets BC3 + full mip chain.

### 4. Convert
Click “Start Conversion”.

Your converted DDS files will appear in the `output/` folder.

---

## 🛠 Building the EXE (Developers)

To generate the EXE using PyInstaller:

1. Enter the directory containing:
   - covex_converter.py
   - icon.ico

2. Run:

rmdir /S /Q build dist 2>nul

pyinstaller ^
  --onefile ^
  --noconsole ^
  --name CovexTextureConverter ^
  --icon=icon.ico ^
  --add-data "icon.ico;." ^
  covex_converter.py

This creates:

dist/CovexTextureConverter.exe

Move it into your release folder alongside:

- texconv.exe
- pngs/
- output/

---

## 🔧 Developer Requirements

If running from source:

pip install PySide6

Python 3.9+ recommended.

---

## 📝 Notes

- The icon is embedded using --add-data and loaded from the PyInstaller bundle.  
- texconv.exe must be shipped next to the main EXE.  
- Conversion uses CREATE_NO_WINDOW to prevent CMD popping up.  
- Drag-and-drop auto-imports PNGs into the pngs/ folder.  
- The UI logs conversion progress and maintains a file count.

---

## 🧵 Support

Want additional features?

- Custom UI themes  
- Auto-updater  
- Texture preview  
- Installer builder  
- New formats or presets  
- New icon / branding

Just open an issue or reach out.

---

© 2025 Covex Studios — All Rights Reserved
