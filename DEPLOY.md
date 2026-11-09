# Yayına alma

Bu klasör Goal Zoo'nun gizlilik politikası ve destek sayfalarıdır. GitHub Pages'te
**oyunun adını taşıyan ayrı bir organizasyondan** yayınlanır; böylece adreste kişisel
isim geçmez.

## Adresler

| Sayfa | Adres |
| --- | --- |
| Privacy Policy (EN) | https://goal-zoo.github.io/ |
| Gizlilik Politikası (TR) | https://goal-zoo.github.io/gizlilik-politikasi/ |
| Help & Support (EN) | https://goal-zoo.github.io/support/ |
| Yardım ve Destek (TR) | https://goal-zoo.github.io/destek/ |

## Adımlar

1. GitHub'da (kendi hesabınla girişliyken) sağ üst **+ → New organization → Free**.
   Ad: **`goal-zoo`**. Üyelikler varsayılan olarak gizlidir; öyle kalsın, böylece
   organizasyon sayfasında adın görünmez.
2. Organizasyonda **public** bir repo aç: **`goal-zoo.github.io`** (ad birebir böyle
   olmalı). README, .gitignore ya da lisans ekleme; repo boş kalsın.
3. Bu klasörde:
   ```
   git remote add origin git@github.com:goal-zoo/goal-zoo.github.io.git
   git push -u origin main
   ```
4. Repo → **Settings → Pages**: Source "Deploy from a branch", `main` / `(root)`.
   `*.github.io` adlı repolarda bu genelde kendiliğinden açıktır.
5. 1–2 dakika sonra dört adresi de tarayıcıda aç. Oyunda Ebeveynler → soruyu
   cevapla → "Gizlilik Politikası" bağlantısı da açılmalı.

Not: commit'lerin yazar adı repo geçmişinde görünür; adresin kendisinde isim yoktur.

## App Store Connect'e yazılacaklar

- **Privacy Policy URL**: İngilizce için `https://goal-zoo.github.io/`, Türkçe için
  `https://goal-zoo.github.io/gizlilik-politikasi/`
- **Support URL**: İngilizce `https://goal-zoo.github.io/support/`, Türkçe
  `https://goal-zoo.github.io/destek/`

Mağaza metinlerinin tamamı oyun reposunda: `goal-zoo/docs/app-store.md`.

## Değiştirirken

- Politika değişirse iki dilde de **yürürlük tarihini** güncelle.
- İletişim adresi dört sayfada da geçiyor (`mailto:`); değişirse hepsinde değiştir.
- Sitede betik, web fontu, analitik ya da çerez olmasın: oyunun "hiçbir şey toplamayız"
  sözü siteyi de kapsar.
