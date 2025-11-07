# 🗓️ RandevuKolayDemo — Akıllı Randevu Yönetim Sistemi (.NET 8)

**RandevuKolay**, işletmelerin randevu oluşturma ve yönetim süreçlerini dijitalleştirmek için geliştirilen modern bir rezervasyon platformudur.  
Proje, **Clean Architecture** prensipleriyle inşa edilmiş olup, **.NET 8** altyapısı, **Entity Framework Core**, **PostgreSQL**, **Hangfire**, **MailKit**, **Identity**, **JWT** ve **FluentValidation** teknolojilerini bir araya getirir.

---

## 🚀 Öne Çıkan Özellikler

- 🔐 **Kimlik Doğrulama & JWT Yetkilendirme**
  - ASP.NET Core Identity ve JWT tabanlı giriş-çıkış işlemleri.
- 🏢 **İşletme Yönetimi**
  - Sektöre göre filtreleme (örnek: kuaför, klinik, tamirhane vb.)
  - Çalışma saatlerini ve hizmetleri yönetme.
- 💇‍♀️ **Hizmet Modülü**
  - Hizmet ekleme (isim, ücret, süre).
  - İşletmeye özel hizmet listesi.
- 📅 **Rezervasyon Yönetimi**
  - Haftalık rezervasyon takvimi görüntüleme.
  - Günlük mesai başlangıcında işletmelere e-posta hatırlatması.
  - Randevu oluşturma, iptal etme, geçmiş görüntüleme.
- ✉️ **Mail Hatırlatma Sistemi**
  - Hangfire ve MailKit ile arka planda otomatik e-posta gönderimi.
- 📊 **Dashboard & Analitik**
  - Chart.js ile haftalık/aylık rezervasyon grafikleri.
- 🧩 **Modern Mimarî**
  - Clean Architecture + Repository Pattern + FluentValidation + AutoMapper.

---

## 🧰 Teknoloji Yığını

### 🔹 Backend
- **.NET 8 Web API**
- **Entity Framework Core 8**
- **PostgreSQL**
- **Hangfire** (Background Job Scheduler)
- **MailKit** (SMTP E-posta Servisi)
- **FluentValidation**
- **AutoMapper**
- **ASP.NET Core Identity**
- **JWT Authentication**

### 🔹 Frontend
- **ASP.NET Core MVC / Razor Pages**
- **Bootstrap 5**
- **Chart.js** (Dashboard grafikler)
- **jQuery + AJAX**

### 🔹 Araçlar
- **Swagger** – API test ve dokümantasyon  
- **Hangfire Dashboard** – Görev kontrol paneli  
- **Postman** – API test aracı  
- **Visual Studio 2022 / Rider**  
- **Git & GitHub**

---

## 🧱 Clean Architecture Katmanları

Proje **Clean Architecture** mimarisine göre yapılandırılmıştır.  
Bu yapı, bağımlılıkları minimuma indirir, test edilebilirliği artırır ve uzun vadede sürdürülebilir kod tabanı oluşturur.
### 🧩 Clean Architecture Katmanları

| Katman | Açıklama |
|--------|-----------|
| **Domain** | Temel iş kuralları, entity’ler ve interface tanımları bulunur. |
| **Application** | Use case’ler, servisler, DTO’lar ve CQRS yapısı yer alır. |
| **Infrastructure** | Veritabanı erişimi, dış servis entegrasyonları (MailKit, Hangfire) bulunur. |
| **API** | Web API katmanı, controller yapısı ve endpoint yönetimi. |
| **UI (MVC)** | Razor tabanlı kullanıcı arayüzü, Dashboard ve görsel yönetim katmanı. |

---
## 📸 Uygulama Görselleri

RandevuKolay arayüzü, kullanıcı dostu ve modern bir tasarıma sahiptir.  
Aşağıda uygulamanın farklı bölümlerine ait ekran görüntülerini inceleyebilirsiniz 👇  

---
### 🏠 Ana Sayfa  
Kullanıcıların hizmet ve işletme bilgilerine kolayca ulaşabildiği modern açılış ekranı.  
<img width="100%" alt="Ana Sayfa" src="assets/Anasayfa.png" />

---

### 🏢 İşletme Detay Sayfası  
İşletmeye ait hizmet, iletişim bilgisi ve randevu oluşturma ekranı.  
<img width="100%" alt="İşletme Detay Sayfası" src="assets/İşletme_Profili.png" />

---

### 🗂️ İşletmeler Sayfası  
Tüm işletmelerin listelendiği, sektör filtrelemesi yapılabilen sayfa.  
<img width="100%" alt="İşletmeler Sayfası" src="assets/İşletmeler_Sayfası.png" />

---

### 📊 Rezervasyon Dashboard  
Chart.js grafikleriyle zenginleştirilmiş haftalık ve aylık rezervasyon analiz ekranı.  
<img width="100%" alt="Rezervasyon Dashboard" src="assets/Rezervasyon_Dashboard.png" />

---

### 📅 Haftalık Randevu Programı  
İşletmelerin haftalık randevularını görüntüleyebildiği dinamik takvim ekranı.  
<img width="100%" alt="Haftalık Randevu Programı" src="assets/Haftalik_Program.png" />

---

### 💇‍♀️ İşletmeye Özel Hizmet Ekleme  
İşletmelerin sundukları hizmetleri (ücret, süre, açıklama) ekleyebildiği sayfa.  
<img width="100%" alt="Hizmet Ekleme Sayfası" src="assets/İşletme_Hizmet.png" />

---

### 👤 Kullanıcı Profili  
Kullanıcıların geçmiş randevularını ve kişisel bilgilerini görüntüleyebildiği alan.  
<img width="100%" alt="Kullanıcı Profili" src="assets/Kullanıcı_Profil.png" />

---

### 🔐 Giriş (Login) Sayfası  
Kimlik doğrulama işlemleri için modern ve responsive giriş ekranı.  
<img width="100%" alt="Login Sayfası" src="assets/Giriş.png" />

---

### 📝 Kullanıcı Kayıt Sayfası  
Yeni kullanıcıların kolayca hesap oluşturabildiği kayıt ekranı.  
<img width="100%" alt="Kullanıcı Kayıt Sayfası" src="assets/Kullanici_kayit.png" />

---

### 🏢 İşletme Kayıt Sayfası  
İşletmelerin kayıt olurken sektör, hizmet türü ve çalışma bilgilerini ekleyebildiği sayfa.  
<img width="100%" alt="İşletme Kayıt Sayfası" src="assets/İşletme_Kayit.png" />

---

### 🗄️ Veritabanı Diyagramı  
Clean Architecture yapısına uygun olarak oluşturulan PostgreSQL veritabanı ilişkileri.  
<img width="100%" alt="Veritabanı Diyagramı" src="assets/DB_diagram.png" />

---

## 🚀 Yakında Hizmete Geçecek

**RandevuKolay**, küçük işletmelerin randevu süreçlerini dijitalleştirerek operasyonel verimliliği artırmayı hedefleyen modern bir rezervasyon platformudur.  
Bu repo, **Emir Adıyaman** tarafından geliştirilen **RandevuKolayDemo** uygulamasını tanıtmaktadır.  

📢 **Canlı sürüm** yayınlandığında, bu sayfada veya ilgili canlı repoda bağlantı paylaşılacaktır.  
Her türlü geri bildirim ve iş birliği teklifleri için [emiradymn.com.tr](https://emiradymn.com.tr) adresinden iletişime geçebilirsiniz.  

✨ **Yakında hizmete geçmesi dileğiyle...**


---
🧾 **Lisans ve Telif Hakkı**

Tüm hakları saklıdır.  
© 2025 **Emir Adıyaman** — Bu proje, Emir Adıyaman tarafından geliştirilmiştir.  
Projenin tasarımı, mimarisi ve içeriği üzerinde tüm fikri ve sınai mülkiyet hakları geliştiriciye aittir.  
İzinsiz kopyalanamaz, çoğaltılamaz veya dağıtılamaz.



