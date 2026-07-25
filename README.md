# Vazifedar — macOS

Kurum içi görev atama ve takip uygulamasının macOS istemcisi.

## İndir

### ⬇️ [Vazifedar.dmg — en son sürüm](https://github.com/hayrat/homebrew-vazifedar/releases/latest/download/Vazifedar.dmg)

Kurulum: indirdiğin DMG'ye çift tıkla, açılan pencerede **Vazifedar**'ı **Uygulamalar** klasörüne sürükle, sonra Uygulamalar'dan aç.

Uygulama Hay Teknoloji'nin Developer ID sertifikasıyla imzalı ve Apple tarafından onaylanmıştır (notarization), bu yüzden açarken güvenlik uyarısı çıkmaz.

**Gereksinim:** macOS 14 (Sonoma) veya üzeri.

### Homebrew ile

Terminal kullanmayı tercih ediyorsan:

```sh
brew tap hayrat/vazifedar
brew trust hayrat/vazifedar
brew install --cask vazifedar
```

Sonraki sürümlere `brew upgrade --cask vazifedar` ile geçersin. (`brew trust`, Homebrew 6'nın üçüncü parti tap'ler için istediği tek seferlik onaydır.)

> Daha önce `hayrat/tap` üzerinden kurduysan: o tap kaldırıldı, cask artık burada.
> `brew untap hayrat/tap` deyip yukarıdaki üç satırı çalıştırman yeterli — uygulamanın
> kendisine dokunulmaz.

## Güncelleme

0.0.2 ve sonrasında uygulama kendini günceller: menü çubuğundaki simge → **Güncellemeleri denetle**. Yeni sürüm varsa indirir, imzasını doğrular ve yeniden başlatır.

0.0.1'de bu özellik henüz yoktu; oradan çıkmak için bir kereliğine yukarıdaki DMG'yi indirmen (ya da `brew upgrade --cask vazifedar`) gerekir.

## Giriş

İki yoldan giriş yapabilirsin:

- **Google ile** — kurum Google hesabınla.
- **E-posta kodu ile** — adresini yaz, gelen 6 haneli kodu gir. Parola yok.

İlk girişten sonra bir kuruma katılman gerekir. Kurum davet kodunu yöneticinden alıp girersin; yönetici onayladıktan sonra görevlerin görünür olur.

## Sürümler

Tüm sürümler [Releases](https://github.com/hayrat/homebrew-vazifedar/releases) sayfasında. Belirli bir sürümü doğrudan indirmek için:

```
https://github.com/hayrat/homebrew-vazifedar/releases/download/macos-0.0.2/Vazifedar.dmg
```

## Kaynak kod

Bu repo yalnız dağıtım içindir — kaynak kod özel bir repoda tutulur.

`Casks/vazifedar.rb` elle düzenlenmez: her sürümde `vazifedar` reposundaki `make macos-cask` tarafından üretilip buraya yazılır. Repo adındaki `homebrew-` öneki Homebrew'in tap kuralı gereğidir; aynı repo hem tap hem indirme sayfasıdır, böylece dağıtım için tek bir public repo yeter.
