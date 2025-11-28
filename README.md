# 🖼️ Covex Texture Converter  
PNG → DDS Converter for FiveM / GTA V  
By Covex Studios

A modern drag‑and‑drop texture converter for FiveM / GTA V using texconv.exe internally.  
Clean UI, dark/light mode, presets, progress bar, and no CMD flashing.

---

## 🚀 Features

- Drag & drop PNG files or folders  
- Batch conversion  
- BC1 / BC3 / BC7 formats  
- FiveM preset (BC3 + full mip chain)  
- Light / Dark theme toggle  
- Real‑time progress bar  
- Silent conversion (no CMD window)  
- Embedded app icon  
- Fully portable (no install)

---

## 📁 Folder Structure (Release)

Your release folder should look like:

```
CovexTextureConverter/
├─ CovexTextureConverter.exe      ← main application
├─ texconv.exe                    ← required conversion engine
├─ pngs/                          ← place PNG files here
└─ output/                        ← converted DDS files appear here
```

Do NOT remove texconv.exe — the converter requires it.

---

## 🧑‍🏫 How to Use

1. **Drag & Drop**  
   Drop PNG files or folders anywhere in the app.  
   They are copied into the `pngs/` folder automatically.

2. **Select Output Format**  
   - BC1_UNORM (no alpha)  
   - BC3_UNORM (FiveM recommended)  
   - BC7_UNORM (high quality)

3. **FiveM Preset**  
   Click “For FiveM preset” to auto‑configure BC3 + full mips.

4. **Convert**  
   Press **Start Conversion**.  
   DDS files appear in the `output/` folder.

---

## 📝 Notes

- Icon is bundled directly inside the EXE.  
- texconv.exe must remain next to CovexTextureConverter.exe.  
- Drag‑and‑drop autofills the `pngs/` folder.  
- Log panel shows all conversion messages.
- Delete the PNGS/DDS thats already in there there placeholders!

---

## 💻 Requirements

- Windows 10 / 11  
- No Python required  
- Portable single‑EXE tool

---

## 🧵 Support

For bugs, feature requests, or enhancements, contact Covex Studios or open a GitHub issue.

© 2025 Covex Studio
