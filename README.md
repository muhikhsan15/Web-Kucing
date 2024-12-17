# Web-Kucing
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website Pencarian Kucing Hilang</title>
    <!-- Google Font -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;600&display=swap" rel="stylesheet">
    <style>
        /* Global Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(to right, #f4a261, #e76f51);
            color: #333;
        }
        /* Navigation */
        nav {
            background-color: #264653;
            display: flex;
            justify-content: center;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
        }
        nav ul {
            display: flex;
            list-style: none;
            padding: 15px;
        }
        nav ul li {
            margin: 0 20px;
        }
        nav ul li a {
            text-decoration: none;
            color: #f4a261;
            font-weight: 600;
            transition: all 0.3s;
        }
        nav ul li a:hover {
            color: #e9c46a;
            transform: scale(1.1);
        }
        /* Section Styles */
        section {
            padding: 60px 10%;
            text-align: center;
        }
        section h1 {
            font-size: 2.5em;
            color: #264653;
            margin-bottom: 15px;
            animation: fadeIn 1s ease-in-out;
        }
        section p {
            font-size: 1.1em;
            margin: 10px 0;
        }
        /* Profile Image */
        .profileImage {
            border-radius: 50%;
            box-shadow: 0px 8px 15px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease-in-out;
        }
        .profileImage:hover {
            transform: scale(1.1);
        }
        /* About and Contact Cards */
        .card {
            background: #fff;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            padding: 20px;
            margin: 20px auto;
            max-width: 600px;
            transition: transform 0.3s;
        }
        .card:hover {
            transform: translateY(-10px);
        }
        /* Contact Section */
        #contact {
            background-color: #2da4a4;
            color: #ffffff;
            text-align: center;
            padding: 60px 20px;
        }
        #contact .card {
            background: #ffffff;
            color: #333;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            padding: 30px;
            max-width: 500px;
            margin: 0 auto;
        }
        #contact .profileImage {
            border-radius: 50%;
            width: 120px;
            height: 120px;
            object-fit: cover;
            margin-bottom: 15px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
        }
        #contact .contact-info p {
            margin: 10px 0;
            font-size: 1.1rem;
        }
        #contact a {
            color: #2da4a4;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s ease-in-out;
        }
        #contact a:hover {
            color: #e76f51;
        }
        /* Footer */
        footer {
            background-color: #264653;
            color: #ffffff;
            text-align: center;
            padding: 20px;
        }
        /* Animation */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        /* Responsive Design */
        @media (max-width: 768px) {
            nav ul {
                flex-direction: column;
                text-align: center;
            }
            section {
                padding: 40px 5%;
            }
            .card {
                padding: 15px;
            }
        }
    </style>
</head>

<body>
    <!-- Background Image -->
    <div class="background"></div>
    
    <!-- Kotak Pencarian -->
    <div class="search-container">
        <input type="text" placeholder="Cari informasi kucing hilang..." class="search-box">
        <button class="search-button">🔍</button>
    </div>

    <!-- Navigation -->
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#biodata kucing">Biodata Kucing</a></li>
            <li><a href="#contact">Contact</a></li>
            <li><a href="#" id="logout">Log Out</a></li>
        </ul>
    </nav>
    <script>
        // Fungsi log out sederhana
        document.getElementById('logout').addEventListener('click', function (e) {
            e.preventDefault();
            
            // Tampilkan konfirmasi log out
            const confirmLogout = confirm('Apakah Anda yakin ingin keluar?');
    
            if (confirmLogout) {
                // Aksi log out (contoh: reset localStorage dan arahkan ke halaman login)
                localStorage.clear(); // Menghapus data sesi pengguna jika disimpan di localStorage
                alert('Anda telah berhasil log out.');
                
                // Arahkan ke halaman login (ubah "login.html" sesuai halaman Anda)
                window.location.href = 'login.html';
            }
        });
    </script>        
</body>

    <!-- Home Section -->
    <section id="home">
        <img class="profileImage" src="assect/image/OIP (3).jpg" alt="Profile Image" width="250">
        <h1>SATU KLIK BISA MEMBAWA MEREKA PULANG!!!</h1>
        <h2>Kucing Hilang? Kami Bisa Membantu!</h2>
        <h3>"Temukan kucing Anda dengan mudah melalui jaringan komunitas pencinta kucing"</h3>
        <h4>Ayoo, Kita Cari!!..</h4>
    </section>

    <!-- Biodata Kucing Section -->
    <section id="biodata kucing">
        <h1>Biodata Kucing</h1>
        <div class="card">
            <img class="image 1" src="assect/image/download.jpg" alt="image 1" width="200">
            <p><strong>Nama Kucing:</strong> kelly</p>
            <p><strong>Umur:</strong> 1 tahun</p>
            <p><strong>Tinggi Kucing:</strong> 15 cm</p>
            <p><strong>Jenis Kelamin:</strong> Laki-laki</p>
            <p><strong>Ciri-ciri:</strong> Ekor Pendek</p>
            <p><strong>Warna Bulu:</strong> Oren, Putih</p>
        </div>
        <div class="card 1">
            <img class="image 2" src="assect/image/OIP.jpg" alt="image 2" width="200">
            <p><strong>Nama Kucing:</strong> Siti</p>
            <p><strong>Umur:</strong> 3 Bulan</p>
            <p><strong>Tinggi Kucing:</strong> 7 cm</p>
            <p><strong>Jenis Kelamin:</strong> Laki-laki</p>
            <p><strong>Ciri-ciri:</strong> Ekor Panjang</p>
            <p><strong>Warna Bulu:</strong> Oren, Putih</p>
        </div>
        <div class="card 2">
            <img class="image 3" src="assect/image/OIP (1).jpg" alt="image 3" width="200">
            <p><strong>Nama Kucing:</strong> Tuyul</p>
            <p><strong>Umur:</strong> 4 Bulan</p>
            <p><strong>Tinggi Kucing:</strong> 10 cm</p>
            <p><strong>Jenis Kelamin:</strong> Betina</p>
            <p><strong>Ciri-ciri:</strong> Tidak Punya Ekor</p>
            <p><strong>Warna Bulu:</strong> Tidak Berbulu</p>
        </div>
        <div class="card 3">
            <img class="image 4" src="assect/image/OIP (2).jpg" alt="image 4" width="200">
            <p><strong>Nama Kucing:</strong> Abigail</p>
            <p><strong>Umur:</strong> 5 Bulan</p>
            <p><strong>Tinggi Kucing:</strong> 10 cm</p>
            <p><strong>Jenis Kelamin:</strong> Betina</p>
            <p><strong>Ciri-ciri:</strong> Ekor Panjang</p>
            <p><strong>Warna Bulu:</strong> Oren, Hitam, Putih</p>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h1>Contact</h1>
        <div class="card">
            <img class="profileImage" src="assect/image/WhatsApp Image 2024-10-08 at 19.48.06.jpeg" alt="Profile Image" width="100">
            
            <!-- Instagram -->
            <div class="contact-item">
                <img src="assect/image/ig.jfif" alt="Instagram" width="25"> <a href="https://www.instagram.com/mhd_ikhsan0001" target="_blank">Instagram: @mhd_ikhsan0001</a>
            </div>

            <!-- Email -->
            <div class="contact-item">
                <img src="assect/image/gmail.jfif" alt="Email" width="20"> <a href="https://mail.google.com/mail/u/0/?hl=en#inbox">Email: mhdikhsan594@gmail.com</a>
            </div>

            <!-- WhatsApp -->
            <div class="contact-item">
                <img src="assect/image/wa.jfif" alt="WhatsApp" width="25"> <a href="https://web.whatsapp.com/" target="_blank">WhatsApp: 0899 2560 997</a>
            </div>

            <!-- TikTok -->
            <div class="contact-item">
                <img src="assect/image/tiktok.jfif" alt="TikTok" width="15"> <a href="https://www.tiktok.com/@lucas02066/video/7381033345125240085?is_from_webapp=1&sender_device=pc&web_id=7449176472050992648" target="_blank">TikTok: TanpaNama15</a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 M. Ikhsan | Jangan Panik!!! Ini yang Harus Kamu Lakukan Jika Kucing Hilang</p>
    </footer>
</body>

<body>
    <!-- Elemen audio dengan loop -->
    <audio id="kucing-sound" src="assect/audio/Suara Kucing 2.mpeg" autoplay loop></audio>

    <script>
        // Script untuk memastikan audio otomatis berputar
        document.addEventListener('DOMContentLoaded', function () {
            const catSound = document.getElementById('kucing-sound');

            // Mulai memutar audio jika diblokir browser
            const playAudio = () => {
                catSound.play();
                document.removeEventListener('click', playAudio); // Hapus listener setelah audio berjalan
            };

            // Tambahkan interaksi pertama jika autoplay diblokir
            document.addEventListener('click', playAudio);
        });
    </script>
</body>
</html>
