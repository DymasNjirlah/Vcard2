<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kartu Saya</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .vcard {
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            padding: 20px;
            text-align: center;
            max-width: 400px;
            width: 90%;
            transition: all 0.3s ease;
        }
        .vcard img {
            border-radius: 50%;
            width: 150px;
            height: 150px;
        }
        .vcard h1 {
            margin: 15px 0;
            font-size: 24px;
        }
        .vcard p {
            font-size: 16px;
            color: #666;
        }
        .vcard a {
            display: inline-block;
            margin: 10px 5px;
            text-decoration: none;
            color: #fff;
            background-color: #007BFF;
            padding: 10px 20px;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }
        .vcard a:hover {
            background-color: #0056b3;
        }
        .fade-in {
            opacity: 0;
            transition: opacity 1s ease-in-out;
        }
        .fade-in.show {
            opacity: 1;
        }

        /* Media Queries */
        @media (max-width: 768px) {
            .vcard {
                padding: 15px;
            }
            .vcard h1 {
                font-size: 20px;
            }
            .vcard p {
                font-size: 14px;
            }
            .vcard img {
                width: 120px;
                height: 120px;
            }
        }

        @media (max-width: 480px) {
            .vcard {
                padding: 10px;
            }
            .vcard h1 {
                font-size: 18px;
            }
            .vcard p {
                font-size: 12px;
            }
            .vcard img {
                width: 100px;
                height: 100px;
            }
            .vcard a {
                padding: 8px 15px;
                font-size: 14px;
            }
        }
    </style>
    <!-- Link ke Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
    <div class="vcard fade-in">
        <img src="fotosaya.jpg" alt="My Picture" class="fade-in">
        <h1 class="fade-in">Dimas</h1>
        <p class="fade-in">Siswa SMP PGRI CEPEDAK</p>
        <p class="fade-in">14 year old student, learn writing, learn programming, learn web design, learn cyber C&S, and learn editing.</p>
        
        <div class="fade-in">
            <a href="https://youtube.com/@dimflr?si=FtO4tA1kLx_mP2zJ" target="_blank" class="fade-in">
                <i class="fab fa-youtube"></i> YouTube
            </a>
            <a href="https://www.facebook.com/dimas.oy.12382" target="_blank" class="fade-in">
                <i class="fab fa-facebook"></i> Facebook
            </a>
            <a href="https://www.instagram.com/call.medym?igsh=YzljYTk1ODg3Zg==" target="_blank" class="fade-in">
                <i class="fab fa-instagram"></i> Instagram
            </a>
        </div>
        <a class="contact fade-in" href="https://wa.me/6281236216420" target="_blank">
            <i class="fab fa-whatsapp"></i> Kontak via WhatsApp
        </a>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const fadeElements = document.querySelectorAll('.fade-in');
            fadeElements.forEach(element => {
                element.classList.add('show');
            });
        });
    </script>
</body>
</html>
