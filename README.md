# 🐉 Maceracı Tavernası (BG3 Themed Forum & Quest Board)

Maceracı Tavernası, Baldur's Gate 3 (BG3) karanlık fantezi evreninden ilham alınarak tasarlanmış, kullanıcıların sohbet edebileceği (Forum) ve görev ilanları paylaşabileceği (Quest Board) dinamik bir web projesidir.

Proje, tamamen modern web standartları ile geliştirilmiş olup arka planda kimlik doğrulama (Authentication) ve veritabanı (Database) işlemleri için **Supabase** altyapısını kullanmaktadır.

## 🔮 Özellikler

*   **🎲 Karanlık Fantezi Tasarımı:** Zindan kahverengisi, BG3 altını ve kan kırmızısı tonlarında tamamen sürükleyici bir arayüz.
*   **📜 Taverna Sohbetleri (Forum Sistemi):** Maceracıların "fısıltılarını" (yorumlarını) ve hikayelerini paylaşabileceği ana sohbet alanı.
*   **⚔️ Görev Panosu (Quest Board):** Lonca veya parti arayan maceracıların staj/iş ilanları bırakabileceği dinamik ilan sistemi.
*   **🛡️ Karakter Yaratma (Kayıt & Giriş Sistemi):** Supabase Auth destekli güvenli kayıt ve giriş sistemi. Kullanıcılar profil fotoğrafı ve maceracı adıyla kayıt olabilirler.
*   **📱 Tam Uyumlu (Responsive):** İster devasa bir parşömenden (Masaüstü), ister cebinizdeki ufak bir kristalden (Mobil) kusursuz görünüm.

## 🛠️ Teknolojiler ve Altyapı

*   **Frontend:** HTML5, CSS3 (Vanilla), JavaScript (ES6)
*   **Backend & Veritabanı:** Supabase (PostgreSQL)
*   **Bağımlılıklar (CDN):** `@supabase/supabase-js`
*   **Tipografi:** Google Fonts (`Cinzel` ve `Lora`)

## 🗺️ Sayfa Haritası

Klasik web terimleri yerine projenin ruhuna uygun fantezi terimleri kullanılmıştır:

*   `index.html` - **Ana Giriş:** Maceracıların tavernanın kapısından girdiği ilk sayfa.
*   `tavern.html` - **Taverna:** Ana forum ve sohbet bölümü.
*   `quest-board.html` - **Görev Panosu:** İş ve staj ilanlarının paylaşıldığı pano.
*   `sending-stone.html` - **Ulak Gönderin:** İletişim bilgileri ve büyülü haberleşme kanalları.
*   `camp-rest.html` - **Kampa Dön (Giriş Yap):** Mevcut maceracıların sisteme giriş yaptığı sayfa.
*   `character-creation.html` - **Karakter Yaratma (Kayıt Ol):** Yeni bir hesaba kayıt olma sayfası.
*   `tavern-rules.html` - **Kurallar:** Tavernada uyulması gereken lonca kuralları.

## ⚙️ Kurulum ve Supabase Entegrasyonu

Bu projeyi kendi ortamınızda çalıştırmak için bir Supabase projesine ihtiyacınız vardır:

1.  **Projeyi Klonlayın:** Dosyaları bilgisayarınıza indirin.
2.  **Supabase Projesi Oluşturun:** [Supabase.com](https://supabase.com) üzerinden yeni bir proje başlatın.
3.  **Veritabanını Hazırlayın:** Supabase SQL Editor'de aşağıdaki tabloları oluşturun:
    *   `tavern_posts` (Taverna Konuları)
    *   `tavern_replies` (Fısıltılar/Yorumlar)
    *   `quest_board` (Görevler)
    *(Gerekli SQL kodları için proje geçmişindeki `supabase_kurulum.md` dosyasına bakabilirsiniz)*
4.  **Bağlantı Bilgilerini Girin:** `app.js` dosyası içerisindeki `SUPABASE_URL` ve `SUPABASE_ANON` değişkenlerine kendi Supabase API bilgilerinizi yapıştırın.
5.  **Tarayıcıda Açın:** `index.html` dosyasına çift tıklayarak serüvene başlayın!

---

*“Yolun açık olsun maceracı, kılıcın keskin, büyün kudretli olsun!”* 🎲
