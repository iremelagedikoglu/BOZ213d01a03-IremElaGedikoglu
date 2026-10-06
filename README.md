# BOZ213d01a03-IremElaGedikoglu

## Açık Kaynak Lisans Sözleşmeleri ve Seçim Kriterleri

### 1. GitHub'da Lisans Sözleşmesi Nedir ve Neden Gereklidir?
Bir yazılım projesini lisans eklemeden GitHub'a yüklemek, telif hakkı mevzuatına göre kodun varsayılan olarak **"Tüm Hakları Saklıdır" (All Rights Reserved)** statüsünde kalmasına neden olur. Yani kod depoda herkes tarafından görüntülenebilir olsa dahi yasal olarak başkaları tarafından kopyalanamaz, değiştirilemez veya başka projelerde kullanılamaz. Açık kaynak lisansları (Open Source Licenses), geliştiricinin mülkiyet haklarını korurken üçüncü şahıslara yazılımı kullanma, değiştirme ve dağıtma hakkını yasal bir zeminde sunan sözleşmelerdir. Ayrıca tüm açık kaynak lisansları yazar için bir sorumluluk reddi (no-warranty) sağlayarak olası yazılımsal zararlara karşı hukuki koruma sağlar.

---

### 2. Temel Lisans Türleri ve Aralarındaki Farklar

Açık kaynak lisansları temel olarak iki ana grupta toplanır:

#### A. İzin Verici (Permissive) Lisanslar
Yazılımcıya ve kullanıcılara neredeyse sınırsız özgürlük tanıyan, kodun kapalı kaynaklı veya ticari yazılımlara entegre edilmesine olanak sağlayan lisanslardır.

* **MIT Lisansı:**
  * **Özellikleri:** Açık kaynak ekosisteminin en sade, en kısa ve en yaygın lisansıdır.
  * **İzinler:** Kod serbestçe kullanılabilir, değiştirilebilir, dağıtılabilir ve ticari projelerde kapalı kaynak olarak satılabilir.
  * **Şartı:** Orijinal telif hakkı ve lisans metni yazılımın tüm kopyalarında aynen korunmalıdır.
* **Apache 2.0 Lisansı:**
  * **Özellikleri:** MIT gibi izin vericidir ancak daha kapsamlı hukuki koruma sunar.
  * **Farkı:** Açık bir **patent hakkı devri (patent grant)** içerir. Projeye katkı verenlerin veya şirketlerin, sonradan yazılımı kullananları patent ihlaliyle dava etmesini yasal olarak engeller.

#### B. Telif Feragatli / Korumacı (Copyleft) Lisanslar
Yazılımın ve ondan türetilen tüm yeni projelerin de daima açık kaynak kalmasını zorunlu kılan lisanslardır.

* **GNU General Public License v3 (GPL v3):**
  * **Özellikleri:** Güçlü korumacı (Strong Copyleft) lisanstır.
  * **Kuralı:** GPL lisanslı bir kod kullanılarak geliştirilen veya bu kodla harmanlanan her yeni projenin de zorunlu olarak **GPL v3 ile lisanslanması ve kaynak kodunun herkese açık paylaşılması gerekir**. Kod kapalı kaynaklı ticari bir ürüne dönüştürülemez.
* **GNU Lesser General Public License (LGPL v3):**
  * **Özellikleri:** Zayıf korumacı (Weak Copyleft) lisanstır; çoğunlukla yazılım kütüphaneleri için tercih edilir.
  * **Farkı:** Kapalı kaynaklı projelerin bu kütüphaneyi dinamik olarak bağlamasına (link etmesine) izin verir; yalnızca kütüphanenin kendi kaynak kodunda bir değişiklik yapılırsa o değişikliklerin açık kaynak kalması zorunludur.

---

### 3. Hangi Lisans Hangi Durumda Seçilir?

* **Geniş Kitleler ve Kolaylık (MIT):** Kodun herkes tarafından, ticari firmalar dahil hiçbir yasal engele takılmadan serbestçe kullanılması istendiğinde tercih edilir. Akademik ödevler ve küçük/orta ölçekli araçlar için idealdir.
* **Kurumsal Projeler ve Patent Güvencesi (Apache 2.0):** Şirketlerin katkı sunduğu ve patent davalarından korunmanın öncelikli olduğu büyük çaplı yazılımlarda seçilir.
* **Topluluk ve Açıklığın Korunması (GNU GPL v3):** Koddan faydalanılarak üretilen her yeni çalışmanın da toplulukla paylaşılmasını ve kodun asla tekelleşip kapatılmamasını sağlamak istendiğinde seçilir.
* **Genel Kütüphane Geliştirme (GNU LGPL v3):** Geliştirilen kütüphanenin kapalı kaynaklı ticari uygulamalar tarafından da kullanılabilmesi ancak kütüphanenin kendi bütünlüğünün açık kalması istendiğinde seçilir.

---

### 4. GitHub'da Lisans Nasıl Seçilir?
1. **Yeni Depo Oluştururken:** Depo açma sayfasındaki *"Lisans ekle (Add a license)"* menüsünden istenen lisans şablonu (MIT, Apache 2.0, GPL vb.) doğrudan seçilerek otomatik olarak eklenir.
2. **Var Olan Depoya Eklerken:** Depo ana sayfasında *"Add file > Create new file"* seçilip dosya adı kutusuna `LICENSE` yazıldığında GitHub otomatik bir şablon seçici (*Choose a license template*) butonu sunar; buradan istenen lisans seçilerek depoya taahhüt (commit) edilir.
