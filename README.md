# Praktikum 3: CSS Dasar

**Nama:** Lucky Danang Aryeswara  
**Mata Kuliah:** Pemrograman Web  
**Universitas:** Universitas Pelita Bangsa  

---

## Langkah-Langkah Praktikum

1. **Membuat File HTML (`lab2_css_dasar.html`)**  
   Membuat struktur dasar dokumen HTML yang berisi elemen `<header>`, `<nav>`, dan `<div>` dengan ID `intro`.

2. **Mendeklarasikan Internal CSS**  
   Menambahkan tag `<style>` di dalam tag `<head>` untuk mengatur font pada `body`, border pada `header`, serta tata letak judul `h1`.

3. **Menambahkan Inline CSS**  
   Menerapkan atribut `style="..."` langsung pada tag `<p>` di dalam elemen `#intro` untuk mengatur teks menjadi rata tengah dan mengubah warna teks.

4. **Membuat External CSS (`style_eksternal.css`)**  
   Membuat file stylesheet terpisah untuk mengatur styling navigasi (`nav`), warna latar belakang saat hover, serta menghubungkannya ke HTML menggunakan tag `<link>`.

5. **Menerapkan ID & Class Selector**  
   Menambahkan ID selector `#intro` untuk mengatur area utama serta class selector `.button` dan `.btn-primary` untuk membuat tombol kustom.

---

## Pertanyaan dan Tugas

### 1. Eksperimen Properti & Nilai CSS
*Melakukan percobaan dengan mengubah atau menambahkan properti dan nilai (value) pada file CSS sesuai panduan CSS Cheat Sheet.*

### 2. Perbedaan Pendeklarasian `h1 {...}` dan `#intro h1 {...}`
* **`h1 {...}` (Element Selector):** Berlaku untuk **seluruh** elemen `h1` di dalam dokumen HTML.
* **`#intro h1 {...}` (Descendant Selector):** Hanya berlaku untuk elemen `h1` yang berada di dalam pembungkus dengan ID `intro` (`<div id="intro">`).

### 3. Prioritas CSS Internal, External, dan Inline
Jika ketiga metode digunakan pada elemen yang sama, **Inline CSS** memiliki prioritas tertinggi dan akan ditampilkan di browser, diikuti oleh Internal CSS, lalu External CSS.
* **Contoh:**
  ```html
  <!-- External CSS: p { color: green; } -->
  <!-- Internal CSS: p { color: blue; } -->
  <p style="color: red;">Teks ini akan berwarna Merah</p>