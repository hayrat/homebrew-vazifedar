# Vazifedar — macOS

Kurum içi görev atama ve takip uygulamasının macOS istemcisi.

## İndir

### ⬇️ [Vazifedar.dmg — en son sürüm](https://github.com/hayrat/vazifedar-downloads/releases/latest/download/Vazifedar.dmg)

Kurulum: indirdiğin DMG'ye çift tıkla, açılan pencerede **Vazifedar**'ı **Uygulamalar** klasörüne sürükle, sonra Uygulamalar'dan aç.

Uygulama Hay Teknoloji'nin Developer ID sertifikasıyla imzalı ve Apple tarafından onaylanmıştır (notarization), bu yüzden açarken güvenlik uyarısı çıkmaz.

**Gereksinim:** macOS 14 (Sonoma) veya üzeri.

### Homebrew ile

Terminal kullanmayı tercih ediyorsan:

```sh
brew tap hayrat/tap
brew trust hayrat/tap
brew install --cask vazifedar
```

Sonraki sürümlere `brew upgrade --cask vazifedar` ile geçersin. (`brew trust`, Homebrew 6'nın üçüncü parti tap'ler için istediği tek seferlik onaydır.)

## Giriş

İki yoldan giriş yapabilirsin:

- **Google ile** — kurum Google hesabınla.
- **E-posta kodu ile** — adresini yaz, gelen 6 haneli kodu gir. Parola yok.

İlk girişten sonra bir kuruma katılman gerekir. Kurum davet kodunu yöneticinden alıp girersin; yönetici onayladıktan sonra görevlerin görünür olur.

## Sürümler

Tüm sürümler [Releases](https://github.com/hayrat/vazifedar-downloads/releases) sayfasında. Belirli bir sürümü doğrudan indirmek için:

```
https://github.com/hayrat/vazifedar-downloads/releases/download/macos-0.0.1/Vazifedar.dmg
```

## Kaynak kod

Bu repo yalnız dağıtım içindir — kaynak kod özel bir repoda tutulur.
