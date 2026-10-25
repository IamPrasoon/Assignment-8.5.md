
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Photo Gallery</title>
<style>
* { box-sizing: border-box; }
body { margin: 0; font-family: Arial; }

.container {
    display: grid;
    grid-template-areas:
        "header"
        "main"
        "footer";
    grid-template-columns: 1fr;
    min-height: 100vh;
}
header {
    grid-area: header;
    background: navy;
    color: white;
    padding: 20px;
    text-align: center;
}
main { grid-area: main; padding: 20px; min-width: 0; }

.gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(min(100%, 200px), 1fr));
    gap: 20px;
}
.card {
    background: #eee;
    padding: 10px;
    border-radius: 10px;
    min-width: 0;
    overflow-wrap: anywhere;
    text-align: center;
}
.card img {
    width: 100%;
    height: 180px;
    object-fit: cover;
    border-radius: 8px;
}
footer {
    grid-area: footer;
    background: navy;
    color: white;
    padding: 20px;
    text-align: center;
}
</style>
</head>
<body>
<div class="container">
    <header>
        <h1>My Photo Gallery</h1>
        <p>Beautiful Nature Collection</p>
    </header>

    <main>
        <h2>Gallery</h2>
        <div class="gallery">
            <div class="card">
                <img src="images/1.jpg" alt="Mountains">
                <h3>Mountains</h3>
            </div>
            <div class="card">
                <img src="images/2.jpg" alt="Forest">
                <h3>Forest</h3>
            </div>
            <div class="card">
                <img src="images/3.jpg" alt="Beach">
                <h3>Beach</h3>
            </div>
            <div class="card">
                <img src="images/4.jpg" alt="Sunset">
                <h3>Sunset</h3>
            </div>
            <div class="card">
                <img src="images/5.jpg" alt="River">
                <h3>River</h3>
            </div>
            <div class="card">
                <img src="images/6.jpg" alt="Flowers">
                <h3>Flowers</h3>
            </div>
        </div>
    </main>

    <footer>
        <p>&copy; 2026 Prasoon Anand</p>
    </footer>
</div>
</body>
</html>
