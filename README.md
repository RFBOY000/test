<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="1.css">
   
<body>


<div>
<nav>
    <div class=""><img src="th-removebg-preview (1).png" alt="logo"></div>

<ul>                                
<li>
    <a href="#home">HOME</a></li>
<li>
    <a href="#info">ABOUT</a></li>
<li>
    <a href="#con">content</a></li>




</ul>




</nav>
</div>

<section id="home" class="HOME">
    <div class="Home-con">
        <h1>Selamat datang di website kami</h1>
        
        <button><a href="#info"><h3>Selamat berbelanja</h3></a></button>

   


    </div>
</section>

<section class="info">
<div id="info">




    <h2>Tentang web ini</h2>
    <p>anda bisa menanyakan  informasih yang di inginkan di bawah</p>

</div>
	
<form id="myForm">
    <label for="name">Nama:</label>
    <input type="text" id="name" name="name" required>

    <label for="message">Pesan:</label>
    <textarea id="message" name="message" rows="4" required></textarea>

    <button type="button" onclick="sendWhatsAppMessage()">Kirim</button>
</form>

</div>

</section>
<script>
    function sendWhatsAppMessage() {
        var name = document.getElementById('name').value;
        var message = document.getElementById('message').value;

        // Ganti nomor WhatsApp dan pesan sesuai kebutuhan Anda
        var phoneNumber = '+6281356280939';
        var waMessage = 'Halo, saya ' + name + '. ' + message;

        // Buka aplikasi WhatsApp dengan pesan yang telah ditentukan
        window.location.href = 'https://web.whatsapp.com/' + phoneNumber + '?text=' + encodeURIComponent(waMessage);
    }
</script>
</html>
