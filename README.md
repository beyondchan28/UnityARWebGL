# UnityARWebGL
Project Augmented Reality (AR) menggunakan Unity 

## Scan untuk di redirect ke hasil project
![Link webpage](ar_link.png?raw=true) 

## Arahkan kamera ke sini
![Link webpage](target.jpg?raw=true)

> Swipe menggunakan dua jari untuk me-rotate object.

### Penjelasan Pembuatan
Project dikerjakan menggunakan ZapparSDK for Unity. Jadi, semua pekerjaan yang dibutuhkan untuk setup AR di WebGL telah di handle oleh SDK ini. Sehingga, yang perlu saya lakukan adalah mengikuti dokumentasi dari [official website](https://duckduckgo.com) dan tutorial dari [channel YouTube](https://www.youtube.com/@ZapparApp). Lalu, untuk rotasi input, saya menggunakan [Lean Touch](https://assetstore.unity.com/packages/tools/input-management/lean-touch-30111).

Overview Pengerjaan/Step-By-Step:
- Install Zappar SDK
- Tambahkan ZapparRearCamera ke Scene
- Train Image tracker menggunakan Zappar Editor Tool
- Tambahkan ZapparImageTracker ke Scene
- Set image ke image yang telah di-train
- Tambahkan 3D model sebagai Child dari ZapperImageTracker
- Setup LeanTouch untuk rotasi object
- Setup Web Build
- Pilih Zapper WebGL Template di `Project Settings > Player > Resolution and Presentation`
- Tekan `Update Project Setting to Publish` di Zapper Editor Tool
- Setup compression `Project Settings > Player > Other Settings` ke gz dan centang opsi `Decompression Fallback`
- Project siap di build dan publish

> NOTE: Sebelumnya, saya mencoba menggunakan [Vuforia](https://developer.vuforia.com/home), namun setelah project berhasil dibuat, SDK ini tidak menyediakan support WebGL. Dan sejauh ini, saya juga tidak mendapatkan work around agar AR bisa dijalankan di web.

### Asset yang digunakan
- Cat 3D Model : https://kenney.nl/assets/cube-pets
- Zapper SDK : https://docs.zap.works/universal-ar/unity/getting-started/importing/
- Lean Touch : https://assetstore.unity.com/packages/tools/input-management/lean-touch-30111