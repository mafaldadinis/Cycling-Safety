# Cycling-Safety

> _An Open-Source Smartwatch-based System to Enhance Cyclist Safety_



This repository serves as the umbrella project for the **Cycling Safety** system. It links together all key components as Git submodules:

- [`map_generator`](https://github.com/mafaldadinis/map_generator): Python tool for intersection risk mapping  
- [`TWatch-S3-Cycling-Safety-Firmware`](https://github.com/mafaldadinis/TWatch-S3-Cycling-Safety-Firmware): ESP32-based smartwatch firmware  
- [`Cycling-Safety-App`](https://github.com/mafaldadinis/Cycling-Safety-App): Mobile application for real-time data exchange and user feedback  

---

## 📦 Cloning the Project

To clone the main repo along with **all submodules**, use:

```bash
git clone --recurse-submodules https://github.com/mafaldadinis/Cycling-Safety.git
If you already cloned the repo without submodules:

git submodule update --init --recursive
```
🎯 Initializing Only a Specific Submodule

You can selectively initialize only the submodule(s) you need:

### Clone the main repo (without submodules)
```bash
git clone https://github.com/mafaldadinis/Cycling-Safety.git
cd Cycling-Safety
```
## Initialize just one submodule
```git submodule update --init path/to/submodule```
Example:

```git submodule update --init map_generator```
Other valid paths:
 - ```firmware``` → the ESP32 smartwatch firmware
 - ```app``` → the mobile application
## 🔄 Updating Submodules

To update a submodule to its latest commit on the tracked branch:
```bash
cd map_generator  # or firmware, or app
git checkout main
git pull origin main
```


##📁 Project Structure
```
Cycling-Safety/
├── map_generator/       # Python mapping tools
├── firmware/            # ESP32 smartwatch firmware
├── app/                 # Mobile app (Capacitor/JS)
├── .gitmodules
└── ...
```
