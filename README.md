# AVAVA

AVAVA için bağımlılıksız, statik iletişim sayfası.

- Ana adres: https://www.avava.com.tr/
- İletişim: info@avava.com.tr (`mailto:` bağlantısı ziyaretçinin e-posta uygulamasını açar.)
- GitHub Pages kaynağı: `main` dalı, `/` kök dizini.
- PHP, veritabanı, JavaScript veya derleme adımı gerekmez.

## DNS

Cloudflare DNS üzerinde `www` kaydını `CNAME` türünde `akinayturan.github.io` hedefine yönlendirin. İlk kurulum ve sertifika doğrulaması için **DNS only** kullanın. Aynı isimdeki çakışan A/AAAA/CNAME kayıtlarını değiştirin.

Kök alan adının da www adresine yönlenmesi için `@` A kayıtları:

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

Kök alan adı için eski web A/AAAA kayıtlarını bu yapıyla uyumlu hale getirin. E-posta hizmetinin MX, SPF, DKIM ve DMARC kayıtlarını koruyun.

DNS doğrulandıktan ve sertifika hazır olduktan sonra GitHub deposunda **Settings → Pages → Enforce HTTPS** seçeneğini etkinleştirin.

Resmî rehber: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site

## Yayınlama

`main` dalına gönderilen değişiklikler GitHub Pages tarafından yayımlanır. WordPress yedekleri ve çıkarılmış veritabanı bu depoya dahil edilmez.
