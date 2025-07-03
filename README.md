Harika! İşte size HTML yapısı:
<!DOCTYPE html>
<html>
<head>
  <title>Barışma Teklifi</title>
  <style>
    #kalp {
      width: 200px;
      height: auto;
    }
  </style>
</head>
<body>
  <img id="kalp" src="kalp.jpg" alt="Kalp Fotoğrafı">
  <br>
  <button id="baris">Benimle barışır mısın?</button>
  <button id="barisma">Barışmayı düşünmüyorum</button>

  <script>
    const kalp = document.getElementById("kalp");
    const baris = document.getElementById("baris");
    const barisma = document.getElementById("barisma");
    let boyut = 200;

    baris.addEventListener("click", function() {
      boyut += 20;
      kalp.style.width = boyut + "px";
    });

    barisma.addEventListener("click", function() {
      alert("Peki, anlıyorum...");
    });
  </script>
</body>
</html>

