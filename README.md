# Portofolio Pribadi di GitHub Pages

## A. Langkah-langkah Membuat Repository Baru di GitHub dan Mengaktifkan GitHub Pages

1. **Masuk ke GitHub** melalui [https://github.com](https://github.com).
2. Klik tombol **New Repository** atau buka tautan [https://github.com/new](https://github.com/new).
3. Isi data repository seperti berikut:
   - **Repository name:** `portofolio`
   - **Description:** isi dengan deskripsi singkat (contohnya: "This portfolio was inspired by a tutorial video from Under Ctrl on YouTube...")
   - **Visibility:** pilih **Public**
   - Tambahkan **README file** dan **MIT License** (opsional).
4. Klik tombol **Create repository** untuk membuat repository baru.

<img src="images/create-repo.png">

5. Setelah repository dibuat, upload file proyek kamu seperti `index.html`, `style.css`, dan folder `images`.
6. Pastikan semua file sudah masuk ke branch `main`.

<img src="images/file-repo.png">

7. Buka tab **Settings → Pages**.
8. Di bagian **Build and deployment**, atur sebagai berikut:
   - **Source:** `Deploy from a branch`
   - **Branch:** `main`
   - **Folder:** `/ (root)`
9. Klik **Save**, lalu tunggu hingga muncul tulisan:
   > Your site is live at https://username.github.io/portofolio/

<img src="images/settings-GithubIo.png">

---

## B. Struktur Folder dan File Proyek

Struktur folder dan file yang digunakan dalam proyek portofolio adalah sebagai berikut:

portofolio/
│
├── index.html
├── style.css
├── README.md
└── images/
├── create-repo.png
├── file-repo.png
└── settings-GithubIo.png


### Penjelasan:
- **index.html** → halaman utama website portofolio.  
- **style.css** → file berisi aturan tampilan (warna, font, layout, dll).  
- **README.md** → file dokumentasi berisi penjelasan proyek (file ini).  
- **images/** → folder penyimpanan gambar, termasuk hasil tangkapan layar saat proses pembuatan repository dan pengaturan GitHub Pages.  

Semua file ini diunggah ke repository GitHub agar dapat dideploy ke **GitHub Pages** dan diakses secara publik.

---

## C. Cara Menghubungkan File CSS ke HTML

Agar tampilan dari `style.css` muncul di web, file CSS harus dihubungkan ke HTML menggunakan tag `<link>` di dalam elemen `<head>`.

### Contoh isi file `index.html`
```
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portofolio Pribadi</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <h1>Halo, Saya Tegar</h1>
  <p>Selamat datang di portofolio pribadi saya!</p>
</body>
</html>
```

### Contoh isi file `style.css`
```
body {
  font-family: Arial, sans-serif;
  background-color: #121212;
  color: white;
  text-align: center;
  margin: 0;
  padding: 0;
}

h1 {
  color: #00bfff;
}
```

