# FinCheck 💸

**Kişisel Harcama Takip Uygulaması**

FinCheck, bireylerin harcamalarını kolayca takip edebilmesi için geliştirilmiş bir kişisel finans yönetimi uygulamasıdır.  
Gelir hesaplaması bulunmaz; sadece **gider yönetimi** odaklıdır.

---

## 🎯 Amaç

FinCheck, kullanıcıların aylık giderlerini düzenli olarak kaydedebilmesi, sabit giderlerin otomatik eklenmesi ve geçmiş dönemlere ilişkin düzenlemeleri sınırlı bir şekilde yapabilmesini sağlar.

---

## 🧠 İş Kuralları

### 1. Gider Yönetimi
- Kullanıcılar giderlerini **kategori**, **tutar**, **açıklama**, **tarih** ve **ödeme türü** bilgileriyle kaydeder.  
- **Gelir** girişi yapılmaz; sistem sadece harcama (gider) verilerini işler.

### 2. Sabit Giderler
- Her ay başında tanımlı **sabit giderler** (örneğin kira, fatura, abonelik) sisteme otomatik olarak eklenir.  
- Sabit giderler manuel olarak da düzenlenebilir veya devre dışı bırakılabilir.

### 3. Gider Silme Kuralları
- Bir gider eklendikten sonra **en fazla 3 iş günü** içerisinde silinebilir.  
- 3 iş günü geçtikten sonra gider silme işlemi yapılamaz.

### 4. Gider Güncelleme Kuralları
- Gider bilgileri, ekleme tarihinden itibaren **3 iş günü** boyunca güncellenebilir.  
- Dönem (ay) değiştiğinde, bir önceki döneme ait giderler **yeni ayın ilk 3 iş günü** boyunca da düzenlenebilir.

### 5. Dönem Yönetimi
- Sistem giderleri **aylık dönemler** halinde sınıflandırır.  
- Yeni döneme geçiş, her ayın 1’inde otomatik olarak yapılır.  
- Sabit giderler bu geçişte yeni döneme otomatik olarak aktarılır.

---

## 📅 Örnek Senaryo
- 28 Mart’ta “Elektrik faturası - 450 TL” gideri eklendi.  
- Bu gider 31 Mart’a kadar (3 iş günü) silinebilir.  
- Nisan ayına geçildiğinde, Mart gideri 3 Nisan’a kadar güncellenebilir ancak 4 Nisan’dan itibaren değiştirilemez.

---

## 🧩 Kullanılan Teknolojiler
- **Backend:** Java 21 + Spring Boot  
- **Database (Ana Veriler):** PostgreSQL  
- **Raporlama ve Analiz:** ClickHouse  
- **Frontend:** React + Shadcn UI  
- **Auth:** JWT tabanlı kimlik doğrulama

---

## ⚙️ Gelecek Geliştirmeler
- Harcama istatistikleri (grafikler, kategori bazlı analiz)  
- Limit aşımı uyarı sistemi  
- Aylık raporlama (PDF/Excel çıktısı)  
- E-posta bilgilendirmeleri  
- Kullanıcı bazlı kategori özelleştirmeleri  

---

## 📆 Proje Takvimi
- **Başlangıç Tarihi:** 1 Kasım 2025  
- **Proje Süresi:** 3 ay  
- **Tahmini Bitiş Tarihi:** 31 Ocak 2026

Bu süre zarfında:
- İş kurallarının uygulanması ve gider yönetim modülü tamamlanacak  
- Sabit giderlerin otomatik eklenmesi ve güncelleme/silme mekanizmaları işlevsel olacak  
- Raporlama ve istatistiksel analiz modülleri geliştirilecek  
- Limit aşımı uyarı sistemi ve aylık raporlar hayata geçirilecek

---

## 📄 Lisans
MIT License  
© 2025 FinCheck Project

---
**FinCheck – Harcamalarını fark et, bütçeni yönet.**
