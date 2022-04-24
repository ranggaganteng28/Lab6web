# Tugas Lab 6 Web
## Profil
| # | Biodata |
| -------- | --- |
| **Nama** | Rangga Saputra |
| **NIM** | 312010266 |
| **Kelas** | TI.20.A.2 |
| **Mata Kuliah** | Pemrograman Web |
## 1. Buat file HTML

1. Buat file HTML dengan nama `index.html` .

2. Lalu tambahkan kode dasar HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout</title>
</head>
<body>
    
</body>
</html>
```
## 2. Tambahkan `CSS` dan `JS` bootstrap
Tambahkan css bootstrap didalam tag `<head>`
```html
<!-- Bootstrap CSS -->
<link rel="stylesheet" href="css/style.css">
<link rel="stylesheet" href="css/bootstrap.min.css">
```
Tambahkan js bootstrap didalam tag <body> dibagian bawah
```html
<!-- Bootstrap JS -->
<script src="js/bootstrap.min.js"></script>
```
## 3. Membuat Layout dengan Bootstrap
1. Membuat container dan navigasi
* Tambahkan kode seperti berikut.
```html
<div class="container mt-5">
    <div class="card shadow">
        <h2 class="m-4" style="color: grey;">Layout Sederhana</h2>
        <nav class="navbar navbar-expand-lg navbar-dark bg-primary">
            <div class="container-fluid">
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#">Home</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Artikel</a>
                        </li>
                        <li class="nav-item dropdown">
                            <a class="nav-link" href="#">About</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Kontak</a>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
    </div>
</div>
```
* Maka hasilnya akan seperti ini
![layout](lab6_css_framework/img/layout1.png)
## 2. Membuat section description
```html
<div class="bg-light p-4">
    <h1 class="display-5">Hello, world!</h1>
    <hr class="my-3">
    <p class="my-3">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt incidunt ducimus inventore est aspernatur maxime soluta illo, perferendis dolorum rem dolorem eos nostrum illum consequatur. Error qui illum inventore temporibus!.</p>
    <a class="btn btn-primary btn-lg" href="#" role="button">Learn more</a>
</div>
```
* Tampilanya seperti berikut
![Section](lab6_css_framework/img/section.png)
## 3. Membuat Content I (Card Group)

```html
<!-- Card -->
<div class="row m-0 py-4">
    <div class="col-md-8">
        <div class="row">
            <div class="col-md-4">
                <div class="card w-100 border-light">
                    <div class="card-body text-center">
                        <img src="https://dummyimage.com/120/db7d25/fff.png" alt="" class="rounded-circle mb-3">
                        <h3>Heading</h3> 
                        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Provident, dignissimos?</p>
                        <a href="#" class="btn btn-secondary">View detail</a>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="card w-100 border-light">
                    <div class="card-body text-center">
                        <img src="https://dummyimage.com/120/3e73e6/fff.png" alt="" class="rounded-circle mb-3">
                        <h3>Heading</h3> 
                        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Provident, dignissimos?</p>
                        <a href="#" class="btn btn-secondary">View detail</a>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="card w-100 border-light">
                    <div class="card-body text-center">
                        <img src="https://dummyimage.com/120/71e6d4/fff.png" alt="" class="rounded-circle mb-3">
                        <h3>Heading</h3> 
                        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Provident, dignissimos?</p>
                        <a href="#" class="btn btn-secondary">View detail</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
```

Tampilannya seperti berikut. 
![Card](lab6_css_framework/img/card.png)
### 4. Membuat Content II

```html
<div class="card p-3 mt-4 border-light">
    <div class="card-body">
        <h3 class="text-dark mb-3">First Featurette Heading</h3>
        <div class="row">
            <div class="col-md-3">
                <img src="https://dummyimage.com/150/7b8a70/fff.png" class="rounded" alt="">
            </div>
            <div class="col-md-9">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsum, accusamus.</p>
            </div>
        </div>
    </div>
</div>
<hr class="my-3">
<div class="card p-3 my-4 border-light">
    <div class="card-body">
        <h3 class="text-dark mb-3">First Featurette Heading</h3>
        <div class="row">
            <div class="col-md-9">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsum, accusamus.</p>
            </div>
            <div class="col-md-3">
                <img src="https://dummyimage.com/150/7b8a70/fff.png" class="rounded" alt="">
            </div>
        </div>
    </div>
</div>
```

Tampilannya seperti berikut.
![Content2](lab6_css_framework/img/content2.png)

## 5. Membuat Sidebar

```html
<!-- Sidebar -->
<div class="col-md-3">
    <div class="card mb-3 ">
        <div class="card-header text-white bg-primary fw-bold">
            Widget Header
        </div>
        <ul class="list-group list-group-flush">
            <li class="list-group-item">Widget Link</li>
            <li class="list-group-item">Widget Link</li>
            <li class="list-group-item">Widget Link</li>
            <li class="list-group-item">Widget Link</li>
        </ul>
    </div>
    <div class="card mb-3">
        <div class="card-header text-white bg-primary fw-bold">
            Widget Header
        </div>
        <ul class="list-group list-group-flush">
            <li class="list-group-item">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Reprehenderit similique alias mollitia voluptatum placeat quia illo quasi fuga. Earum, ducimus illo. Iure repellat at adipisci?</li>
        </ul>
    </div>
</div>
```
Tampialnnya seperti berikut. 

![Widget](lab6_css_framework/img/widget.png)
## 6. Membuat Footer

```html
<footer class="bg-dark text-white p-3 text-center">&copy; 2022 - Universitas Pelita Bangsa | Rangga Saputra</footer>
```
![Footer](lab6_css_framework/img/footer.png)

# Sekian Terima Kasih
# Selamat Menjalankan UTS




