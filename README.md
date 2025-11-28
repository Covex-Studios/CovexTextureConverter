===========================================================
                COVEX TEXTURE CONVERTER
          PNG → DDS Converter for FiveM / GTA V
                    By Covex Studios
===========================================================

Covex Texture Converter is a fast, modern drag-and-drop tool
for converting PNG textures into DDS formats commonly used in
FiveM, GTA V, and other DirectX-based engines.

It uses texconv.exe (Microsoft DirectXTex) behind the scenes,
wrapped in a clean dark/light UI with progress bars, presets,
and drag-and-drop support.

-----------------------------------------------------------
FEATURES
-----------------------------------------------------------
✔ Drag & drop PNG files or folders
✔ Batch conversion (hundreds at once)
✔ BC1 / BC3 / BC7 output formats
✔ FiveM preset (BC3 + full mip chain)
✔ Dark / Light theme toggle
✔ Modern UI with Tailwind-style design
✔ Real-time progress bar + detailed log
✔ No flashing CMD window during conversion
✔ Icon fully embedded in the EXE
✔ Fully portable – no installation required

-----------------------------------------------------------
FOLDER STRUCTURE (RELEASE VERSION)
-----------------------------------------------------------
Your release folder should look like this:

CovexTextureConverter/
├─ CovexTextureConverter.exe      ← the app
├─ texconv.exe                    ← required converter engine
├─ pngs/                          ← put PNG files here
└─ output/                        ← DDS files appear here

IMPORTANT:
Do NOT remove texconv.exe – the converter cannot run without it.

-----------------------------------------------------------
HOW TO USE
-----------------------------------------------------------

1. DROP PNGS
Drag & drop PNG files or folders onto the window.
They will be copied into the "pngs" folder automatically.

2. SELECT OUTPUT FORMAT
Choose one:
- BC1_UNORM (no alpha)
- BC3_UNORM (good for FiveM, supports alpha)
- BC7_UNORM (highest quality)

3. APPLY FIVEM PRESET (OPTIONAL)
Click “For FiveM preset”
→ sets BC3 + full mip chain.

4. START CONVERSION
Click “Start Conversion”.

Converted DDS files will appear in the "output" folder.

-----------------------------------------------------------
NOTES
-----------------------------------------------------------
• The icon is embedded in the EXE using PyInstaller.
• texconv.exe must remain next to CovexTextureConverter.exe.
• CMD windows are hidden during conversion (silent mode).
• Drag-and-drop auto-imports PNGs into the "pngs" folder.
• The log panel shows the status of every conversion.

-----------------------------------------------------------
SYSTEM REQUIREMENTS
-----------------------------------------------------------
• Windows 10/11
• No Python required
• No installation required (fully portable)

-----------------------------------------------------------
SUPPORT
-----------------------------------------------------------
For feature requests, UI redesigns, bug reports, or custom
presets, feel free to open an issue or contact Covex Studios.

-----------------------------------------------------------
© 2025 Covex Studios — All Rights Reserved
===========================================================
