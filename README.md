<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="1.css">
   <style>
html{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
    
    }
    body{
    scroll-behavior: smooth;
        background-color: #0a1d28;
    }
    nav{
    background-color: #0a1d28;
    display: flex;
    justify-content: space-between;
    padding: 1rem 2rem;
    position: sticky;
    top:0;
    }
    
    nav ul{
        align-items: center;
        display: flex;
        gap:2rem;
        list-style: none;
        
    }
    nav ul li a{
        font-weight: bold;
        text-decoration: none;
        font-family:"Segoe UI", sans-serif;
        color: whitesmoke;
    }
    nav div img{
        width: 50px;
    }
    
    nav ul li a:hover{
        color:#146C94 ;
    border-bottom: 2px solid aqua;
    }
    
    .HOME{
        height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        background-image: url("download.jpg");    
        
       
    
    }
    .Home-con{
        background-color: transparent;
    max-width: 600px;
    display: flex;
    flex-direction: column; /* agar teks berada di tengah */
    align-items: center;
    justify-content: center;
    text-align: center; /* tambahkan ini agar teks berada di tengah */
    padding: 20px; /* sesuaikan padding sesuai kebutuhan */
    
    }
    .Home-con h1{
        font-size: 56px;
        font-weight: 700;
        color: whitesmoke;
        text-align: center;

        
    }
    .Home-con h3{
        font-size: 32px;
        font-weight: 700;
        color: #00abf0;
        text-align: center;

    }
    .Home-con p{
        color: whitesmoke;
        font-size: 16px;
        font: weight 700px; ;
      
    }
    .Home-con button{ 
        width: 300px;
        height: 150px;
        background-color: #0a1d28;
        border: 2px solid #00abf0;
        border-radius: 10px;
       
       
    }
    .Home-con button a{
        color: #00abf0;
       
       
        font-size: 19px;
        font-weight: 700;
        text-decoration: none;
        letter-spacing: 1px;
    }
    .Home-con button a:hover{
        color:#146C94 ;
    }
    
    
    :root {
        scroll-behavior: smooth;
    }
    
    
    
    .info {
        padding: 180px;
        height: 30%;
        text-align: center;
        background-color: #0a1d28;
        color: whitesmoke;
        font-size: 30px;
      align-items: center;
        
        
    }

   .form-container {
            max-width: 400px;
            margin: 20px auto;
            padding: 20px;
            border: 1px solid #ccc;
            border-radius: 10px;
            background-color: #f9f9f9;
        }

        label {
            display: block;
            margin-bottom: 8px;
        }

        input, textarea {
            width: 100%;
            padding: 8px;
            margin-bottom: 16px;
            box-sizing: border-box;
        }

        button {
            background-color: #4caf50;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
   </style>
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
