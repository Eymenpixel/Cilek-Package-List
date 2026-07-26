# 🚀 Kaya Repository

<div align="center">

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Status](https://img.shields.io/badge/Status-Active-success.svg)]()
[![Platform](https://img.shields.io/badge/Platform-Linux%20%2F%20Custom-blue.svg)]()
[![Apt Compatible](https://img.shields.io/badge/Manager-APT-orange.svg)]()

> *Hazır depoların kısıtlamalarından sıkılanlar için tamamen özgün, kendi ellerimizle kodladığımız çekirdek paket deposu!*

</div>

---

## 📌 Kaya Nedir?
**Kaya**, dışarıdaki standart Ubuntu/Debian depolarına bağımlı kalmadan kendi kurallarımızı koyduğumuz ve `.deb` paketlerimizi barındırdığımız özel `apt` paket deposudur. 

## 📂 Depo Yapısı (`pool` & `dists`)
*   `pool/`: Sistemimize kurulmayı bekleyen `.deb` dosyalarının ve ham paketlerin ana yuvasıdır.
*   `dists/`: `apt` yöneticisinin paketleri okuyabilmesi için gereken indekslerin (`Packages`, `Release` vb.) tutulduğu alandır.

## ⚙️ Depoyu Sisteme Ekleme
Bu depoyu kendi sistemine entegre etmek için `/etc/apt/sources.list` dosyasına şu satırı ekleyebilirsin:
```text
deb [trusted=yes] file:///yol/to/Kaya stable main
