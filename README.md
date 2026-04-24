# SAARJ Template

`SAARJ Template`, akademik dergi makaleleri icin form tabanli LaTeX paketleri ureten masaustu bir aractir. Dergi bilgileri, yazarlar, bolumler, sekil ve tablolar arayuz uzerinden girilir; uygulama da Overleaf'e hazir bir ZIP paketi olusturur.

## Ozellikler

- Dergi adi, ISSN/e-ISSN, URL, logo ve vurgu rengi ozellestirme
- Coklu yazar, kurum, e-posta ve ORCID destegi
- Bolum, alt bolum ve alt-alt bolum olusturma
- Sekil ve tablo ekleme, dosya yukleme ve yerlesim secimi
- Profil kaydetme ve yeniden kullanma
- Overleaf'e hazir `main.tex` ve ek dosyalarla ZIP cikti uretme
- XeLaTeX uyumlu cift dilli kapak ve kaynakca yapisi

## Proje Yapisi

- `app.py`: Flask uygulamasi ve form akisinin endpoint'leri
- `formatter.py`: LaTeX uretimi ve ZIP paketleme mantigi
- `templates/index.html`: tek sayfa form arayuzu
- `.github/workflows/build.yml`: Windows ve macOS paketleme sureci

## Lokal Calistirma

1. Python 3.11+ kurulu olsun.
2. Bagimliliklari yukleyin:

```bash
pip install -r requirements.txt
```

3. Uygulamayi baslatin:

```bash
python app.py
```

4. Tarayicida `http://127.0.0.1:5051` adresini acin.

## Kullanim Akisi

1. Dergi ayarlarini girin veya kayitli bir profil yukleyin.
2. Kapak bilgileri, yazarlar, ozetler ve bolumleri doldurun.
3. Gerekirse sekil, tablo ve ek alanlari ekleyin.
4. `LaTeX Olustur & ZIP Indir` butonuyla Overleaf paketini olusturun.
5. Overleaf'te projeyi yukleyip derleyiciyi `XeLaTeX` olarak secin.

## Notlar

- Uretilen paket, dergi logosu, CC-BY gorseli ve sekilleri ZIP icinde birlikte sunar.
- Profil dosyalari kullanicinin ev dizininde ayri bir klasorde saklanir.
- Varsayilan gorunur marka bu revizyonda `SAARJ Template` olarak duzenlendi; paketleme dosyalarinda eski teknik dosya adlari henuz korunuyor.

## Lisans

[MIT License](LICENSE)

