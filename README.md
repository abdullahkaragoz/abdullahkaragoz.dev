# abdullahkaragoz.dev — PortfolioOS

Bir özgeçmiş sayfası yerine, tarayıcıda açılan küçük bir **masaüstü işletim sistemi** gibi tasarlanmış kişisel portföy. Menü çubuğu, dock ve sürüklenip boyutlandırılabilen pencerelerle gerçek bir masaüstü deneyimi sunar.

🔗 Canlı: **https://abdullahkaragoz.dev**

---

## Özellikler

- **Masaüstü kabuğu:** üst menü çubuğu, saat, dock (büyüteç efektli) ve sürüklenebilir / boyutlandırılabilir / büyütülebilir pencereler.
- **Uygulamalar:** Hakkımda, Deneyim, Projeler, Yetenekler, Eğitim, Sertifikalar, Hobiler, İletişim, CV (PDF görüntüleyici) ve komutlarla gezilebilen bir **Terminal**.
- **Kişiselleştirme:** duvar kâğıdı, vurgu rengi ve dock boyutu seçenekleri; tercihler tarayıcıda saklanır.
- **İki dil:** Türkçe / İngilizce anında geçiş.
- **Mobil uyumlu:** dokunmatik ve dar ekranlar için uyarlanmış arayüz.

## Oyunlar

Dock'taki **Oyunlar** klasöründe (açılır ızgara):

- **Yılan** — klasik snake
- **Road Fighter** — yukarıdan görünümlü yarış
- **Duck Hunt** — özgün nişancı (köpek, uçan ördekler, turlar, skor, sesler)
- **Mayın Tarlası** — birebir Windows görünümlü (7-segment sayaçlar, gülen yüz, chord, uzun-bas ile bayrak)
- **2048** — kaydır-birleştir bulmaca (klasik renk paleti, animasyonlar, en iyi skor)

Tüm oyunlar tek dosyalık, bağımsız ve mobil dokunmatik desteklidir.

## Radyo

Açık **Radio-Browser** dizinini kullanan canlı radyo uygulaması: Türkiye / Popüler / Favoriler sekmeleri, arama, oynat-duraklat, ses, favoriler. İstasyonların kendi herkese açık canlı yayın akışını çalar.

## Teknoloji

- Herhangi bir arayüz kütüphanesi (React/Vue vb.) **kullanılmadan**; saf **JavaScript + HTML + CSS**.
- Pencere/dock/menü mantığı için kendi yazdığım küçük bir bileşen motoru (`support.js`).
- Oyunlarda **HTML5 Canvas**, seste **Web Audio API**.
- Harici bağımlılık yok; tek istisna radyo için açık Radio-Browser API'si (çalışma anında, anahtarsız).

## Çalıştırma

Statik bir sitedir; derleme adımı yoktur.

```bash
# en basit yol: index.html'i tarayıcıda açın
# ya da yerel bir statik sunucu çalıştırın:
python -m http.server 8080
# sonra: http://localhost:8080
```

Herhangi bir statik barındırmada (GitHub Pages, Netlify, Vercel, Cloudflare Pages) yayınlanabilir.

## Proje yapısı

```
.
├── index.html        # masaüstü kabuğu + tüm uygulamalar
├── support.js        # bileşen motoru
├── radio.html        # Radyo uygulaması
├── duck-hunt.html    # Duck Hunt oyunu
├── favicon.svg       # AK favicon
├── game/             # 2048, mayın tarlası, yılan, road fighter
└── assets/           # avatar, CV
```

## Lisans

Kaynak kod **MIT Lisansı** ile lisanslanmıştır — bkz. [LICENSE](LICENSE).

**İstisna:** Kişisel içerik MIT kapsamı dışındadır ve tüm hakları saklıdır — buna fotoğraf (`assets/avatar.jpg`), özgeçmiş (`assets/Abdullah-Karagoz-CV.pdf`), biyografi, deneyim/iletişim metinleri ve "Abdullah Karagöz" kimliğine ait diğer veriler dâhildir. Kodu serbestçe kullanabilir/uyarlayabilirsiniz; lütfen kişisel bilgileri ve kimliği kendi bilgilerinizle değiştirin.

## İletişim

- Web: https://abdullahkaragoz.dev
- LinkedIn: https://www.linkedin.com/in/abdullahkaragoz
- GitHub: https://github.com/abdullahkaragoz

---

### English (short)

A personal portfolio reimagined as a tiny **desktop OS** in the browser — menu bar, dock, draggable/resizable windows. Includes apps (About, Experience, Projects, Skills, CV, Terminal…), a **Games** folder (Snake, Road Fighter, Duck Hunt, a Windows-style Minesweeper, 2048) and a live **Radio** app (open Radio-Browser API). Built with **vanilla JavaScript, HTML and CSS** — no UI frameworks — using HTML5 Canvas and the Web Audio API.

The source code is **MIT licensed** (see [LICENSE](LICENSE)). Personal content — photo, CV, bio and the "Abdullah Karagöz" identity — is **excluded** and all rights reserved; please replace it with your own if you reuse the code.
