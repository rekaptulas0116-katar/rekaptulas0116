  <!DOCTYPE html>
  <html lang="id">
  <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Karang Taruna Rekaptulas</title>
      <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
      <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
      <link href="https://cdn.jsdelivr.net/npm/simplelightbox@2.14.1/dist/simple-lightbox.min.css" rel="stylesheet">
      <style>
          /* Gradasi Latar Belakang Cerah */
          body {
              font-family: 'Roboto', sans-serif;
              background: linear-gradient(to right bottom, #e0f7fa, #bbdefb, #e8f5e9); /* Gradasi Biru Muda, Biru Langit, Hijau Pucat */
              min-height: 100vh; /* Pastikan gradasi menutupi seluruh tinggi viewport */
          }
          header {
              /* PERHATIAN: Pastikan folder yang Anda gunakan di server/repositori adalah 'img' atau ubah ke 'images' jika itu nama foldernya */
              background: url('img/banner.jpg') center/cover no-repeat;
              height: 300px;
              color: white;
              display: flex;
              align-items: center;
              justify-content: center;
              text-align: center;
          }
          header h1 {
              background-color: rgba(0,0,0,0.5);
              padding: 15px;
              border-radius: 10px;
          }
          .logo { max-width: 120px; }
          
          /* --- CSS BARU UNTUK GALERI YANG RAPI --- */
          .gallery-item-container {
              width: 100%;
              height: 200px; /* Tinggi thumbnail seragam */
              overflow: hidden; /* Sembunyikan bagian yang terpotong */
              border-radius: 5px;
              display: block; /* Agar tautan mengambil lebar penuh */
          }
          .gallery-item-container img {
              width: 100%;
              height: 100%;
              object-fit: cover; /* Ini yang membuat gambar mengisi penuh kotak dan terpotong rapi */
              cursor: pointer;
              transition: transform 0.3s ease;
          }
          .gallery-item-container img:hover {
              transform: scale(1.05); /* Efek zoom saat di hover */
          }
          /* --- Akhir CSS BARU --- */

          .category-buttons button { margin: 5px; }
          footer {
              background-color: #333;
              color: white;
              padding: 20px 0;
              text-align: center;
              margin-top: 50px; /* Tambahkan sedikit jarak dari konten atas */
          }

          /* Styling untuk bagian yang disembunyikan/ditampilkan */
          .content-section {
              display: none; /* Default sembunyikan semua bagian konten */
              padding: 30px 0;
              background-color: rgba(255, 255, 255, 0.9); /* Latar belakang semi-transparan untuk konten */
              border-radius: 8px;
              margin-bottom: 20px;
              box-shadow: 0 4px 8px rgba(0,0,0,0.1);
          }
          /* Bagian 'Tentang' akan ditampilkan secara default, jadi override display:none */
          #about.content-section {
              display: block;
          }
      </style>
  </head>
  <body>

  <header>
      <div>
          <img src="img/Cuplikan layar 2025-10-31 000331.jpg" alt="Logo Karang Taruna" class="logo mb-3">
          <h1>Karang Taruna Rekaptulas</h1>
          <p>Alamat: Jl. Cilangkap Rt 001 Rw 016 Kelurahan Cilangkap, Kecamatan Tapos Kota Depok</p>
      </div>
  </header>

  <nav class="navbar navbar-expand-lg navbar-light bg-light sticky-top">
      <div class="container">
          <a class="navbar-brand" href="#">Karang Taruna</a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
              <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarNav">
              <ul class="navbar-nav ms-auto">
                  <li class="nav-item"><button class="nav-link btn btn-link text-decoration-none" data-target="about">Tentang</button></li>
                  <li class="nav-item"><button class="nav-link btn btn-link text-decoration-none" data-target="gallery">Galeri</button></li>
                  <li class="nav-item"><button class="nav-link btn btn-link text-decoration-none" data-target="activities">Kegiatan</button></li>
                  <li class="nav-item"><button class="nav-link btn btn-link text-decoration-none" data-target="contact">Kontak</button></li>
              </ul>
          </div>
      </div>
  </nav>

  <div class="container my-5">
      <section id="about" class="content-section">
          <h2>Tentang Karang Taruna</h2>
          <p>Karang Taruna Rekaptulas adalah organisasi kepemudaan yang bergerak dalam kegiatan sosial, budaya, dan kemasyarakatan yang berlokasi di Jl. Cilangkap Rt 001 Rw 016 Kelurahan Cilangkap, Kecamatan Tapos Kota Depok.</p>
          <p>Kami berkomitmen untuk mengembangkan potensi pemuda dan berkontribusi positif bagi lingkungan sekitar melalui berbagai program dan kegiatan. Visi kami adalah menciptakan pemuda yang mandiri, inovatif, dan berjiwa sosial tinggi.</p>
          <p>Bergabunglah dengan kami untuk menciptakan perubahan positif di komunitas!</p>
      </section>

      <section id="gallery" class="content-section">
          <h2>Galeri Foto Kegiatan</h2>

          <div class="category-buttons mb-3">
              <button class="btn btn-primary" data-filter="all">Semua</button>
              <button class="btn btn-secondary" data-filter="kegiatan Lomba">Lomba</button>
              <button class="btn btn-secondary" data-filter="kegiatan Panggung">Panggung</button>
              <button class="btn btn-secondary" data-filter="kegiatan Sosial">Sosial</button>
          </div>

          <div class="search-bar mb-3">
              <input type="text" id="searchInput" class="form-control" placeholder="Cari kategori kegiatan...">
          </div>

          <div class="row gallery" id="galleryGrid">
              <div class="col-md-3 mb-4" data-category="kegiatan Lomba">
                  <a href="img/IMG_3159.JPG" class="gallery-item-container">
                      <img src="img/IMG_3159.JPG" alt="Kegiatan Lomba">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan Lomba">
                  <a href="img/IMG_3172.JPG" class="gallery-item-container">
                      <img src="img/IMG_3172.JPG" alt="Lomba anak">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan Lomba">
                  <a href="img/IMG_3182.JPG" class="gallery-item-container">
                      <img src="img/IMG_3182.JPG" alt="Lomba anak>
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan Lomba">
                  <a href="" class="gallery-item-container">
                      <img src="" alt="Lomba anak">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan olahraga">
                  <a href="img/[NAMA FILE FOTO 5]" class="gallery-item-container">
                      <img src="img/[NAMA FILE FOTO 5]" alt="Lomba Agustusan">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan budaya">
                  <a href="img/[NAMA FILE FOTO 6]" class="gallery-item-container">
                      <img src="img/[NAMA FILE FOTO 6]" alt="Upacara Bendera">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan sosial">
                  <a href="img/[NAMA FILE FOTO 7]" class="gallery-item-container">
                      <img src="img/[NAMA FILE FOTO 7]" alt="Gotong Royong">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan olahraga">
                  <a href="img/[NAMA FILE FOTO 8]" class="gallery-item-container">
                      <img src="img/[NAMA FILE FOTO 8]" alt="Senam Bersama">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan budaya">
                  <a href="img/[NAMA FILE FOTO 9]" class="gallery-item-container">
                      <img src="img/[NAMA FILE FOTO 9]" alt="Parade Busana">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan sosial">
                  <a href="img/[NAMA FILE FOTO 10]" class="gallery-item-container">
                      <img src="img/[NAMA FILE FOTO 10]" alt="Kunjungan Panti">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan olahraga">
                  <a href="img/[NAMA FILE FOTO 11]" class="gallery-item-container">
                      <img src="img/[NAMA FILE FOTO 11]" alt="Turnamen Voli">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan budaya">
                  <a href="img/[NAMA FILE FOTO 12]" class="gallery-item-container">
                      <img src="img/[NAMA FILE FOTO 12]" alt="Tari Tradisional">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan sosial">
                  <a href="img/[NAMA FILE FOTO 13]" class="gallery-item-container">
                      <img src="img/[NAMA FILE FOTO 13]" alt="Penyuluhan Kesehatan">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan olahraga">
                  <a href="img/[NAMA FILE FOTO 14]" class="gallery-item-container">
                      <img src="img/[NAMA FILE FOTO 14]" alt="Lari Maraton">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan budaya">
                  <a href="img/[NAMA FILE FOTO 15]" class="gallery-item-container">
                      <img src="img/[NAMA FILE FOTO 15]" alt="Lomba Pidato Bahasa Daerah">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan sosial">
                  <a href="img/[NAMA FILE FOTO 16]" class="gallery-item-container">
                      <img src="img/[NAMA FILE FOTO 16]" alt="Santunan Yatim">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan olahraga">
                  <a href="img/[NAMA FILE FOTO 17]" class="gallery-item-container">
                      <img src="img/[NAMA FILE FOTO 17]" alt="Turnamen Badminton">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan budaya">
                  <a href="img/[NAMA FILE FOTO 18]" class="gallery-item-container">
                      <img src="img/[NAMA FILE FOTO 18]" alt="Nonton Bareng Film Nasional">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan sosial">
                  <a href="img/[NAMA FILE FOTO 19]" class="gallery-item-container">
                      <img src="img/[NAMA FILE FOTO 19]" alt="Membersihkan Lingkungan">
                  </a>
              </div>

              <div class="col-md-3 mb-4" data-category="kegiatan olahraga">
                  <a href="img/[NAMA FILE FOTO 20]" class="gallery-item-container">
                      <img src="img/[NAMA FILE FOTO 20]" alt="Lomba Egrang">
                  </a>
              </div>

                      </div>
      </section>

      <section id="activities" class="content-section">
          <h2>Kegiatan Terbaru</h2>
          <ul>
              <li>**01 Januari 2025:** Kegiatan Sosial: Bakti Sosial pembagian sembako kepada warga kurang mampu.</li>
              <li>**15 Februari 2025:** Kegiatan Budaya: Pentas seni tradisional dan modern tingkat desa.</li>
              <li>**20 Maret 2025:** Kegiatan Olahraga: Turnamen sepak bola antar RW memperebutkan Piala Bergilir Karang Taruna.</li>
              <li>**10 April 2025:** Lingkungan: Gerakan bersih-bersih lingkungan dan penanaman pohon.</li>
              <li>**05 Mei 2025:** Pendidikan: Workshop keterampilan digital untuk pemuda.</li>
          </ul>
      </section>

      <section id="contact" class="content-section">
          <h2>Kontak Kami</h2>
          <p>Jika Anda memiliki pertanyaan, saran, atau ingin berpartisipasi dalam kegiatan kami, jangan ragu untuk menghubungi:</p>
          <p><strong>Email:</strong> <a href="mailto:rekaptulas0116@gmail.com">rekaptulas0116@gmail.com</a></p>
          <p><strong>Telepon/WhatsApp:</strong> <a href="https://wa.me/6281281948632" target="_blank">+62-812-8194-8632</a></p>
          <p><strong>Instagram:</strong> <a href="https://www.instagram.com/rekaptulas_id" target="_blank">@rekaptulas_id</a></p>
          <p>Kami akan dengan senang hati membantu Anda!</p>
      </section>
  </div> 

  <footer>
      <p>&copy; 2025 Karang Taruna Rekaptulas. All rights reserved.</p>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/simplelightbox@2.14.1/dist/simple-lightbox.min.js"></script>
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script> 

  <script>
      // Lightbox init
      if (typeof jQuery !== 'undefined') {
          var lightbox = new SimpleLightbox('.gallery a', { /* options */ });
      } else {
          console.warn("jQuery not loaded, SimpleLightbox might not work as expected.");
      }

      // Category Filter Buttons
      const filterButtons = document.querySelectorAll('.category-buttons button');
      let galleryItems = document.querySelectorAll('#galleryGrid .col-md-3'); 
      
      filterButtons.forEach(btn => {
          btn.addEventListener('click', () => {
              const filter = btn.getAttribute('data-filter');
              
              galleryItems = document.querySelectorAll('#galleryGrid .col-md-3'); 
              
              galleryItems.forEach(item => {
                  if(filter === 'all' || item.getAttribute('data-category') === filter) {
                      item.style.display = '';
                  } else {
                      item.style.display = 'none';
                  }
              });
              // Highlight active button
              filterButtons.forEach(b => {
                  b.classList.remove('btn-primary');
                  b.classList.add('btn-secondary');
              });
              btn.classList.remove('btn-secondary');
              btn.classList.add('btn-primary');
          });
      });

      // Search Filter
      const searchInput = document.getElementById('searchInput');
      searchInput.addEventListener('input', function() {
          const filter = searchInput.value.toLowerCase();
          
          galleryItems = document.querySelectorAll('#galleryGrid .col-md-3');
          
          galleryItems.forEach(item => {
              const category = item.getAttribute('data-category').toLowerCase();
              if(category.includes(filter)) {
                  item.style.display = '';
              } else {
                  item.style.display = 'none';
              }
          });
      });

      // --- Custom JS for showing/hiding sections ---
      const navButtons = document.querySelectorAll('.navbar-nav .nav-item .btn');
      const contentSections = document.querySelectorAll('.content-section');

      navButtons.forEach(button => {
          button.addEventListener('click', function() {
              const targetId = this.getAttribute('data-target');

              // Sembunyikan semua bagian konten
              contentSections.forEach(section => {
                  section.style.display = 'none';
              });

              // Tampilkan bagian konten yang sesuai dengan tombol yang diklik
              const targetSection = document.getElementById(targetId);
              if (targetSection) {
                  targetSection.style.display = 'block';
              }

              // Opsional: Gulir ke bagian yang ditampilkan
              targetSection.scrollIntoView({ behavior: 'smooth', block: 'start' });

              // Opsional: Hapus kelas 'active' dari semua tombol nav
              navButtons.forEach(btn => btn.classList.remove('active'));
              // Tambahkan kelas 'active' ke tombol yang sedang diklik (jika ingin menonjolkan)
              this.classList.add('active');
          });
      });

      // Inisialisasi: Pastikan 'Tentang' aktif dan ter-highlight saat halaman dimuat
      document.addEventListener('DOMContentLoaded', () => {
          document.querySelector('.navbar-nav .nav-item .btn[data-target="about"]').classList.add('active');
      });

  </script>

  </body>
  </html>
