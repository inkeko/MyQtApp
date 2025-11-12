# MyQtApp

Ez egy egyszerű Qt GUI alkalmazás, amelyet C++ és Qt 6.10 segítségével fejlesztettem Visual Studio Code-ban, MinGW fordítóval.

## 🛠️ Fejlesztési környezet

- Qt 6.10.0 (MinGW 64-bit)
- CMake 3.27+
- Visual Studio Code
- MinGW 13.1.0
- GDB debugger
- Windows 11

## 📁 Projekt struktúra
MyQtApp/ 
── main.cpp
 ├── CMakeLists.txt
  ├── .vscode/           # VS Code konfigurációk 
  ├── build/             # CMake build mappa (gitignore-ozva) 
  ├── dist/              # Futtatható fájlok és Qt DLL-ek 
  └── README.md



## ⚙️ Build és futtatás

1. **CMake konfigurálás**  
   `Ctrl + Shift + P` → `CMake: Configure`

2. **Fordítás**  
   `Ctrl + Shift + P` → `CMake: Build`

3. **Futtatás**  
   `F5` → automatikusan fut a `windeployqt`, majd indul az alkalmazás

## 🚀 Terjesztés

A `dist/` mappa tartalmazza:

- `MyQtApp.exe`
- Qt DLL-ek (`Qt6Core.dll`, `Qt6Widgets.dll`, stb.)
- `platforms/` mappa (`qwindows.dll`)

Ez a mappa ZIP-be csomagolható, és másik gépen is futtatható Qt telepítés nélkül.

## 📦 Verziókezelés

A projekt `.gitignore` fájlja kizárja a `build/`, `dist/` és ideiglenes fájlokat. Csak a forráskód és a konfigurációk kerülnek fel GitHubra.

## ✨ Tervek

- GUI bővítése gombokkal, szövegmezőkkel
- Reusable Qt sablon létrehozása
- Dokumentáció bővítése

---
