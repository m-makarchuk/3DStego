<div align="center">
  <h1>3DStego</h1>

  <p>
    <img src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Android" />
    <img src="https://img.shields.io/badge/Kotlin-B125EA?style=for-the-badge&logo=kotlin&logoColor=white" alt="Kotlin" />
    <img src="https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white" alt="Rust" />
    <img src="https://img.shields.io/badge/License-Apache_2.0-blue.svg?style=for-the-badge" alt="License" />
  </p>

</div>

## 🏆 About the Project

<p align="justify">
  <b>3DStego</b> is an autonomous mobile software suite designed for advanced steganographic data protection. By integrating the geometry of 3D models with graph spectral analysis, it provides a highly secure and robust method for hiding data within 3D objects. The embedded data remains highly resilient to affine transformations.
</p>

## ⚙️ Architecture & Tech Stack

<p align="justify">
  The application features a hybrid architecture designed to maximize computational performance while minimizing memory footprint on mobile devices:
</p>

<ul>
  <li><div align="justify"><b>User Interface:</b> Built natively for Android using <b>Kotlin</b> following the MVVM architectural pattern.</div></li>
  <li><div align="justify"><b>Computational Core:</b> Developed in <b>Rust</b> to efficiently handle heavy mathematical operations and spectral analysis.</div></li>
  <li><div align="justify"><b>Integration:</b> Communication between the Kotlin UI and the Rust core is implemented via a <b>JNI bridge</b> using <b>Zero-Copy technology</b>, ensuring zero overhead during large data transfers.</div></li>
  <li><div align="justify"><b>3D Rendering:</b> Powered by <b>Google Filament</b> for high-quality, real-time visualization of 3D models on mobile devices.</div></li>
</ul>

## 🔐 Algorithms & Cryptography

<ul>
  <li><div align="justify"><b>Spectral Decomposition:</b> Utilizes the <b>Lanczos algorithm</b> to optimize the spectral decomposition of graphs, drastically improving processing times for complex 3D meshes.</div></li>
  <li><div align="justify"><b>Encryption:</b> All payload data is strictly secured using <b>AES-256-GCM</b> cryptographic encryption <i>before</i> the steganographic embedding process begins.</div></li>
</ul>

## 📥 Installation (APK Release)

<p align="justify">
  Currently, 3DStego is available as a pre-compiled Android package (<code>.apk</code>).
</p>

<ol>
  <li><div align="justify">Navigate to the <a href="../../releases">Releases</a> section of this repository.</div></li>
  <li><div align="justify">Download the latest <code>3DStego.apk</code> file to your Android device.</div></li>
  <li><div align="justify">Open the downloaded file. <i>(Note: You may need to enable "Install unknown apps" in your Android security settings)</i>.</div></li>
  <li><div align="justify">Follow the on-screen instructions to install and launch the application.</div></li>
</ol>

## 🗺️ Roadmap & Open Source

<p align="justify">
  This project is built with a strict commitment to <b>Free and Open Source Software (FOSS)</b> principles.
</p>
<p align="justify">
  Currently, only the compiled APK is available in this repository for testing and demonstration purposes. The complete source code (both the Kotlin UI and the Rust core libraries), along with detailed build instructions for Android Studio and Cargo, is being prepared for a full public release in the near future.
</p>

## 📄 License

<p align="justify">
  Once the source code is published, this project will be licensed under the <b>Apache License 2.0</b>.
</p>
