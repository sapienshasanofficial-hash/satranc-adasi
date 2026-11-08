# Satranç Adası

4–7 yaş çocuklarına satranç taşlarının hareketini öğreten Android oyunu.

- Paket adı: `com.satrancadasi`
- Oyun: `www/index.html` (tek sayfa), sesler: `www/sesler/` (104 Türkçe cümle, yapay zekâ ile üretildi)
- Uygulama kabuğu: Capacitor 8; satın alma: Google Play Billing (`@capgo/native-purchases`), ürün kimliği `tam_surum`
- Derleme: her `main` gönderiminde GitHub Actions imzasız `.aab` ve telefonda denemek için hata ayıklama `.apk`'sı üretir, ikisini `derlemeler` dalına koyar.
- İmza: `.aab` yükleme anahtarıyla depo dışında (`jarsigner`) imzalanıp Play Console'a yüklenir. Yükleme anahtarı bu depoda ya da GitHub'da hiç bulunmaz.
