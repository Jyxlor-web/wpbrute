💥 Araç Ne Yapıyor?
🎯 Hedef:
Belirli bir WordPress siteye, belirttiğin kullanıcı adıyla, şifre listesinden teker teker deneyip giriş yapmaya çalışıyor.

🔧 Nasıl Çalışıyor?
🖼️ Banner: Güzel ASCII art + Telegram reklamı gösteriyor.

📥 Input Alıyor:

WordPress login adresi (https://site.com/wp-login.php)

Kurulum🔴

```git clone https://github.com/Jyxlor-web/wpbrute.git```

```cd wpbrute```

```python3 wpbrute.py```


Kullanıcı adı

Şifre listesi (pass.txt gibi)

🔁 Her Şifreyi Tek Tek Deniyor

Giriş formunu doldurur gibi POST isteği atıyor

Eğer başarılı giriş olursa, çerezde wordpress_logged_in_ yakalıyor

Veya başarılı yönlendirme durumunu kontrol ediyor (/wp-admin/)

✅ Şifreyi bulursa ekrana yazıyor

❌ Hiçbir şifre çalışmazsa: "başarısız" diyor

⚙️ Teknik Özellikler:
requests.Session() ile cookie yönetimi aktif

Hatalarda otomatik try-except ile devam eder

Tüm girişleri gerçek form gibi gönderir (bot gibi değil)

User-Agent sabit ama istenirse randomlaştırılabilir

🧠 Ne İşe Yarar?
Kendi sistemini test etmek istiyorsan (pentest) ✔️

WordPress’te zayıf şifre kontrolü yapmak için ✔️

Güvenlik açıkları/zayıflıkları olan demo sitelerde eğitim amaçlı kullanılabilir

⚠️ Uyarı:
🔴 Bu tool'u sadece izinli testlerde, kendi sitende veya lab ortamında kullanmalısın.
İzinsiz kullanımı yasal değildir ve suç teşkil eder.
