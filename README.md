# SiberAI API ve yerel ajan kaynakları

SiberAI adına hazırlanmıştır. Bu depo, [SiberAI](https://siberai.net/) resmi dokümantasyonuna giden kısa, olgusal bir başlangıç notudur. Kod çalıştırılmamış, canlı API çağrısı yapılmamıştır.

## SiberAI nedir?

SiberAI; Siber v3 modeli, OpenAI uyumlu API ve yerel kod ajanını kod inceleme, güvenlik analizi ve hata ayıklama iş akışlarında bir araya getirir.

## API sabitleri

| Ayar | Değer |
| --- | --- |
| Temel adres (`base_url`) | `https://siberai.net/api/siberai/v1` |
| Model kimliği | `siber-v3` |
| Anahtar | Ortam değişkeninden okuyun (ör. `SIBERAI_API_KEY`); depoya yazmayın |

Erişim geçerli hesap, çalışma alanı yetkisi ve yeterli bakiye gerektirir. Kullanım token tüketimine göre ücretlendirilir; güncel fiyat için [fiyatlandırma](https://siberai.net/pricing) sayfasına bakın.

## Yerel ajan

- Windows ve Linux x64 geliştirme paketleri sunulur.
- Native ajan bir işletim sistemi sandbox'ı değildir; araçlar kullanıcının işletim sistemi yetkileriyle çalışır.
- Öneriler insan incelemesi ve testle doğrulanmalıdır.

## Kontrol listesi

1. `base_url` tam olarak SiberAI adresini mi gösteriyor?
2. Model alanı `siber-v3` mü?
3. Anahtar secret store'da mı, loglarda görünmüyor mu?
4. Hata alındığında HTTP durumu ve hata kodu birlikte okunuyor mu?

## Resmî kaynaklar

- [Ana sayfa](https://siberai.net/)
- [Hızlı başlangıç](https://siberai.net/docs/quickstart)
- [Kimlik doğrulama](https://siberai.net/docs/authentication)
- [Hata kodları](https://siberai.net/docs/errors)
- [Yerel ajan](https://siberai.net/docs/agent)
- [Güvenlik](https://siberai.net/security)
- [Güvenlik analizi kullanım senaryosu](https://siberai.net/use-cases/security-analysis)
