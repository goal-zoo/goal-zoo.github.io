# Yayına alma

Bu klasör Goal Zoo'nun gizlilik politikası ve destek sayfalarıdır (oyunun 15 dilinin her
biri için ikişer sayfa). **Sayfalar burada elle düzenlenmez:** oyun reposundaki `site/`
klasöründen `node scripts/site.mjs` ile yazılır; bu klasöre yalnızca bitmiş dosyalar gelir.
GitHub Pages'te `goal-zoo` organizasyonundan yayınlanır (`main` dalı, kök klasör); `main`'e
gönderilen her şey 1–2 dakikada yayına girer.

**Bu repo herkese açıktır.** Sayfalardaki iletişim adresi geliştiricinin destek adresidir
(oyun reposunda `site/config.mjs` → `CONTACT`). Sayfalara, commit'lere ve bu dosyaya başka
kişisel bilgi ya da başka uygulamaların adı yazılmaz.

## Adresler

| Dil | Gizlilik politikası | Yardım ve destek |
| --- | --- | --- |
| English | https://goal-zoo.github.io/ | https://goal-zoo.github.io/support/ |
| Türkçe | https://goal-zoo.github.io/gizlilik-politikasi/ | https://goal-zoo.github.io/destek/ |
| diğer 13 dil | `https://goal-zoo.github.io/<dil>/` | `https://goal-zoo.github.io/<dil>/support/` |

`<dil>`: `es`, `pt`, `de`, `fr`, `it`, `id`, `ru`, `ar`, `hi`, `ja`, `ko`, `zh-hans`,
`zh-hant`. Her sayfanın başındaki 🌐 menüsü aynı sayfanın öbür dillerine götürür.

## Her push'tan önce

1. Oyun reposunda `node scripts/site.mjs`, ardından `node scripts/site.mjs --check`:
   "0 differ" demeli (bu klasör kaynaklarla aynı).
2. Birkaç sayfayı yerelde tarayıcıda aç (dosyayı çift tıklamak yeter).
3. `git push`; 1–2 dakika sonra adresleri kontrol et (en az İngilizce, Türkçe ve bir de
   Arapça: sağdan sola). Oyunda Ebeveynler → soruyu cevapla → "Gizlilik Politikası"
   bağlantısı da açılmalı.

## App Store Connect'e yazılacaklar

Her mağaza yerelleştirmesi kendi dilinin iki adresini alır (yukarıdaki tablo). Adresler ve
bütün mağaza metinleri oyun reposunda hazır durur: `goal-zoo/store/metadata/<locale>/`
(`privacy_url.txt`, `support_url.txt`); adımlar `goal-zoo/docs/app-store.md`.

## Değiştirirken

Kaynaklar oyun reposundadır: `site/content/<dil>/` (metinler), `site/config.mjs` (adresler,
iletişim adresi, politikanın tarihi), `site/site.css`. Değişiklikten sonra orada
`node scripts/site.mjs`; buradaki dosyalara elle dokunma (bir sonraki çalıştırmada silinir).

- Politika değişirse `site/config.mjs` içindeki `UPDATED` tarihini yayına aldığın günün
  tarihi yap: her dildeki **Son güncelleme** satırı o dilin biçimiyle yeniden yazılır.
- Bütün diller aynı şeyi söylemeli: bir cümle değişirse 15 dilin hepsinde değişir (oyun
  reposundaki test, sayfaların İngilizceyle aynı bloklardan oluştuğunu denetler; cümlenin
  kendisini denetleyemez).
- Türkçe ve İngilizce dışındaki sayfalar çeviridir; sonlarında "fark olursa İngilizce sürüm
  geçerlidir" notu vardır.
- Politika, destek e-postalarının en geç 12 ay içinde silindiğini söylüyor: posta kutusunu
  buna göre temizle. Süreyi değiştirirsen her dildeki politikada da değiştir.
- Oyunun cihazda sakladıkları değişirse (yeni bir ayar, satın alma…) önce politikadaki
  tabloyu her dilde güncelle.
- Sitede betik, web fontu, analitik ya da çerez olmasın: oyunun "hiçbir şey toplamayız"
  sözü siteyi de kapsar. Dil menüsü betiksizdir (HTML `details`).
- Sayfaların başındaki logo oyunun logosudur (`logo.png`: oyunun gösterdiği resmin kopyası;
  sitenin simgeleri de aynı logodan). Logo değişirse oyun reposunda `node scripts/site.mjs`
  logoyu ve bütün sayfaları, `node scripts/brand.mjs --site=../goal-zoo.github.io` simgeleri
  günceller.
