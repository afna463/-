# -
พร้อม เพลย์อัฟนาน
<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<title>ช่องทางการชำระเงิน</title>
<style>
body {
  font-family: sans-serif;
  background: #f5f5f5;
  text-align: center;
  padding: 20px;
}
.gallery {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 15px;
  max-width: 600px;
  margin: auto;
}
.gallery img {
  width: 100%;
  border-radius: 12px;
  cursor: pointer;
}
.lightbox {
  display: none;
  position: fixed;
  inset: 0;
  background: rgba(0,0,0,0.85);
  justify-content: center;
  align-items: center;
}
.lightbox img {
  max-width: 90%;
  max-height: 90%;
}
</style>
</head>
<body>

<h2>ช่องทางการชำระเงิน</h2>

<div class="gallery">
  <img src="img1.jpg" onclick="openImg(this.src)">
  <img src="img2.jpg" onclick="openImg(this.src)">
  <img src="img3.jpg" onclick="openImg(this.src)">
  <img src="img4.jpg" onclick="openImg(this.src)">
</div>

<div class="lightbox" id="lightbox" onclick="this.style.display='none'">
  <img id="lightbox-img">
</div>

<script>
function openImg(src){
  document.getElementById("lightbox-img").src = src;
  document.getElementById("lightbox").style.display = "flex";
}
</script>

</body>
</html>
