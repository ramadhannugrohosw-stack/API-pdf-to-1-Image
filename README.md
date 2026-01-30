# PDF to Long JPG API

API Node.js untuk mengubah **PDF multi-halaman** menjadi **1 file gambar JPG panjang**  
(halaman digabung ke bawah: page 1 → page 2 → dst).

✔ Output **hanya 1 image**  
✔ Cocok untuk preview, OCR, AI Vision, dan pipeline n8n  
✔ Support Windows & Linux (Ubuntu)

---

## ✨ Fitur
- Upload PDF (`multipart/form-data`)
- Render setiap halaman dengan **Ghostscript**
- Gabungkan semua halaman menjadi **1 JPG panjang**
- Support path file **mengandung spasi**
- Bisa atur DPI & kualitas gambar
- Tidak menghasilkan ZIP

---


Cek:
```bash
node -v
npm -v
```

```bash
npm install
npm i sharp
```

```bash
npm start
```


```bash
curl.exe -X POST "http://localhost:3000/v1/convert/pdf-to-jpg" ^
  -F "file=@\"D:\Documents\contoh pdf\rekening.pdf\";type=application/pdf" ^
  -o "D:\Documents\contoh pdf\rekening-LONG.jpg"
```

