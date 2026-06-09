# Kapıdan Önce — Legal site (Privacy + Support)

Bu klasör, App Store için gereken **Gizlilik Politikası** ve **Destek** sayfalarını içerir.
GitHub Pages'te yayınlanmak üzere hazır, bağımsız HTML dosyalarıdır (dış bağımlılık yok).

- `index.html` → Gizlilik Politikası (TR/EN)
- `destek.html` → Destek / Support (TR/EN)

## Yayınlama (GitHub Pages) — 4 adım

1. GitHub'da **yeni, PUBLIC bir repo** aç: örn. `kapidanonce-legal`
   (⚠️ Uygulama kaynağını buraya koyma — sadece bu 2 HTML dosyası.)
2. Bu klasördeki dosyaları o repoya yükle. Terminalden:
   ```sh
   cd ~/Desktop/kapidanonce-site
   git init && git add . && git commit -m "Privacy + support pages"
   git branch -M main
   git remote add origin https://github.com/<KULLANICI_ADIN>/kapidanonce-legal.git
   git push -u origin main
   ```
3. Repo → **Settings → Pages** → "Build and deployment" → Source: **Deploy from a branch**,
   Branch: **main**, klasör: **/ (root)** → **Save**.
4. ~1 dakika sonra adresler hazır olur:
   - Gizlilik: `https://<KULLANICI_ADIN>.github.io/kapidanonce-legal/`
   - Destek:   `https://<KULLANICI_ADIN>.github.io/kapidanonce-legal/destek.html`

## Sonra
- Her iki linki **Safari'de aç, açıldığını doğrula**.
- Gizlilik URL'ini bana ver → uygulamada `AppLinks.privacyPolicy`'ye koyayım.
- App Store Connect:
  - **App Privacy → Privacy Policy URL** = gizlilik linki
  - **App Information → Support URL** = destek linki

## Düzenleme
İletişim e-postası `kemalcansu@icloud.com` ve ad "Kapıdan Önce" olarak yazıldı.
Değiştirmek istersen iki HTML dosyasında geçen bu değerleri güncelle (ve `mailto:` linkini).
