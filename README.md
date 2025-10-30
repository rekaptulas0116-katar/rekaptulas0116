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
        .gallery img { width: 100%; height: auto; border-radius: 5px; cursor: pointer; }
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
            <button class="btn btn-secondary" data-filter="kegiatan sosial">Sosial</button>
            <button class="btn btn-secondary" data-filter="kegiatan budaya">Budaya</button>
            <button class="btn btn-secondary" data-filter="kegiatan olahraga">Olahraga</button>
        </div>

        <div class="search-bar mb-3">
            <input type="text" id="searchInput" class="form-control" placeholder="Cari kategori kegiatan...">
        </div>

        <div class="row gallery" id="galleryGrid">
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
</div> <footer>
    <p>&copy; 2025 Karang Taruna Rekaptulas. All rights reserved.</p>
</footer>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/simplelightbox@2.14.1/dist/simple-lightbox.min.js"></script>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script> <script>
    // Generate 100 gallery images automatically
    const galleryGrid = document.getElementById('galleryGrid');
    const categories = ['kegiatan sosial', 'kegiatan budaya', 'kegiatan olahraga'];
    for(let i=1; i<=100; i++){
        const category = categories[i % 3]; // rotasi kategori
        const div = document.createElement('div');
        div.className = 'col-md-3 mb-4';
        div.setAttribute('data-category', category);
        div.innerHTML = `<a href="img/foto${i}.jpg"><img src="img/foto${i}.jpg" alt="${category}"></a>`;
        galleryGrid.appendChild(div);
    }

    // Lightbox init
    // Pastikan jQuery dimuat sebelum SimpleLightbox jika menggunakan SimpleLightbox.jquery.min.js
    if (typeof jQuery !== 'undefined') {
        var lightbox = new SimpleLightbox('.gallery a', { /* options */ });
    } else {
        console.warn("jQuery not loaded, SimpleLightbox might not work as expected.");
    }


    // Category Filter Buttons
    const filterButtons = document.querySelectorAll('.category-buttons button');
    const items = document.querySelectorAll('#galleryGrid .col-md-3');
    filterButtons.forEach(btn => {
        btn.addEventListener('click', () => {
            const filter = btn.getAttribute('data-filter');
            items.forEach(item => {
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
        items.forEach(item => {
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
    // Ini memastikan tombol 'Tentang' juga memiliki kelas 'active' jika diinginkan
    document.addEventListener('DOMContentLoaded', () => {
        document.querySelector('.navbar-nav .nav-item .btn[data-target="about"]').classList.add('active');
    });

</script>

</body>
</html>
