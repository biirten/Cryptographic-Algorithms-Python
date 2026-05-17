# Cryptographic-Algorithms-Python
# Python ile Kriptografik Şifreleme Uygulamaları (AES, DES & RSA)

Bu proje, modern siber güvenlik ve veri güvenliği standartlarında sıkça kullanılan **Simetrik** ve **Asimetrik** şifreleme algoritmalarının Python dilinde çalışan temiz uygulama örneklerini içerir. Bilgisayar mühendisliği eğitimim kapsamında veri gizliliği ve kriptografi mantığını pratik etmek amacıyla geliştirilmiştir.

---

##  İçerik ve Kullanılan Algoritmalar

Proje kapsamında tek bir çatı altında toplanan 3 ana şifreleme yöntemi bulunmaktadır:

### 1. AES-256 Şifreleme (`aes_encryption.py`)
* En güvenli simetrik şifreleme standartlarından biri olan **AES-256 (Advanced Encryption Standard)** mimarisi uygulanmıştır.
* Veri güvenliğini artırmak amacıyla **CBC (Cipher Block Chaining)** modu kullanılmıştır.
* Her şifrelemede rastgele bir **IV (Initialization Vector - Başlatma Vektörü)** üretilir ve verilerin blok boyutuna uyması için **Padding (Doldurma)** mekanizması entegre edilmiştir.

### 2. DES Şifreleme (`des_encryption.py`)
* Klasik blok şifreleme yöntemlerinden **DES (Data Encryption Standard)** algoritmasının çalışma mantığını simüle eder.
* 8-baytlık (64-bit) anahtar yapısı ve CBC modu kullanılarak şifreleme ve şifre çözme adımları gerçekleştirilmiştir.

### 3. RSA Asimetrik Şifreleme (`rsa_encryption.py`)
* Açık anahtarlı şifreleme yöntemi olan **RSA** algoritması kullanılmıştır.
* Güvenli mimari standartlarına uygun olarak **2048-bit** uzunluğunda asimetrik anahtar çiftleri (Public & Private Key) otomatik olarak üretilir.
* Şifreleme ve imzalama güvenliği için **PKCS1_OAEP** dolgu standardı entegre edilmiştir.

---

##  Teknolojiler ve Kütüphaneler

* **Programlama Dili:** Python 3.x
* **Temel Kütüphane:** `pycryptodome` (Kriptografik işlemler için kullanılan modern Python paketi)
* **Yardımcı Araçlar:** `base64` (Şifreli verilerin güvenli iletimi ve gösterimi için), `os` (Rastgele anahtar üretimi için)

---

##  Nasıl Çalıştırılır?

Projeyi yerel bilgisayarınızda test etmek için gerekli kütüphaneyi yüklemeniz yeterlidir:

```bash
pip install pycryptodome
python aes_encryption.py
python des_encryption.py
python rsa_encryption.py
