# 3DStego
Mobile steganographic data protection app based on 3D model geometry and graph spectral analysis. Core in Rust, UI in Kotlin.

## 🏆 About the Project
**3DStego** is an autonomous mobile software suite designed for advanced steganographic data protection. By integrating the geometry of 3D models with graph spectral analysis, it provides a highly secure and robust method for hiding data within 3D objects. The embedded data remains highly resilient to affine transformations.

## ⚙️ Architecture & Tech Stack
The application features a hybrid architecture designed to maximize computational performance while minimizing memory footprint:

* **User Interface:** Built natively for Android using **Kotlin** following the MVVM architectural pattern.
* **Computational Core:** Developed in **Rust** to efficiently handle heavy mathematical operations and spectral analysis.
* **Integration:** The communication between the Kotlin UI and the Rust core is implemented via a **JNI bridge** using **Zero-Copy** technology, ensuring zero overhead during large data transfers.
* **3D Rendering:** Powered by **Google Filament** for high-quality, real-time visualization of 3D models on mobile devices.

## 🔐 Algorithms & Cryptography
* **Spectral Decomposition:** Utilizes the **Lanczos algorithm** to optimize the spectral decomposition of graphs, drastically improving processing times for complex 3D meshes.
* **Encryption:** All payload data is strictly secured using **AES-256-GCM** cryptographic encryption before the steganographic embedding process begins.

## 🚀 Getting Started

### Prerequisites
To build and run this project locally, you will need:
* Android Studio (latest stable release)
* Rust toolchain (`rustup`, `cargo`)
* Android NDK and CMake (can be installed via Android Studio SDK Manager)

### Build Instructions
1. Clone the repository:
   ```bash
   git clone [https://github.com/m-makarchuk/3DStego.git](https://github.com/m-makarchuk/3DStego.git)
   cd 3DStego
2. Make sure you have the required Rust targets for Android:
   ```bash
   rustup target add aarch64-linux-android armv7-linux-androideabi x86_64-linux-android

3.Open the project in Android Studio. Gradle will automatically trigger the Cargo build for the Rust core libraries during the project sync.

4. Build and run the app on your physical device or emulator.

📄 License

This project is licensed under the Apache License 2.0 - see the LICENSE file for details. Built with a commitment to Free and Open Source Software principles.
