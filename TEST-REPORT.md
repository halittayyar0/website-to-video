# Website to Video — test raporu

31 Ekim 2026. Yerel Windows/Codex ortamında yapıldı. Belge desteği, dosya kurulumu, elle davranış testi ve başka istemcide gerçek çalıştırma ayrı değerlendirilir.

## Gerçekte yapılanlar

Skill Creator doğrulayıcısı ortak çekirdek ve yeni yerel `%USERPROFILE%/.codex/skills/website-to-video` kurulumu için `Skill is valid!` döndürdü. Yeni oturumun menü keşfi test edilmedi. Bu oturum çekirdek dosyalarını okuyarak akışı uyguladı. OpenAI ve Claude resmî kurulum belgeleri açıldı. Claude web/Code kurulumu veya çalıştırması yapılmadı; prompt-only dal Codex'te elle değerlendirildi. GitHub hesabı `halittayyar0` doğrulandı; Chrome'da depo formu erişilebilir, yerel `gh` bulunmuyor. Yayın sonucu ayrı DELIVERY dosyasında kaydedilir.

Her vakada tek iş girdisi URL idi; ek müşteri brief'i verilmedi. Test için yetenek dalı elle seçildi. Bunlar bağımsız taze-model benchmark koşuları değil, skill'in bu oturumda elle yürütülen uçtan uca denemeleridir.

| Vaka | Kanıt | Sonuç |
| --- | --- | --- |
| Tatil kiralama | [Naples](examples/naples.md): ana sayfa, ilgili mülk sayfası ve gerçek avlu fotoğrafı | Tek koleksiyon konsepti, iki eksiksiz İngilizce prompt, sabit mimari ve yalnız su hareketi incelendi. Fotoğrafın belirli ilana eşlemesi doğrulanmadığından o ilanın özelliği gibi kullanılmadı. Prompt-only inceleme geçti; resim üretilmedi. |
| E-ticaret | [Peak Design](examples/peak-design.md): ürün sayfası ve resmî fotoğraf | Prompt-only çıktı/motion planı incelendi. Gerçek üretimde START ve START-referanslı END, ardından iki onarım denendi; kumaş deseni korunamadı. Başarılı ürün resmi testi sayılmadı; kusurlu çiftin reddi uygulandı. |
| Yazılım | [Linear](examples/linear/RESULT.md): ana sayfa, planlama sayfası, gerçek Chrome görünümü | Soyut iş akışı olarak etiketli iki resim gerçekten üretildi; END için START bağlandı. Üç kart, altı çizgi, bağlayıcı ve tek işaret korunuyor. Küçük 2D hareket uygulanabilir. Görsel araçlı yol geçti; gerçek UI/özellik uydurulmadı. |
| Erişim hatası | [Gerçek .invalid isteği](examples/unreachable.md) | Araç erişim hatası döndürdü; marka/üretim uydurulmadan erişilebilir kaynak istendi. Beklenen hata davranışı geçti. |
| Enjeksiyon | [Sentetik metin değerlendirmesi](examples/injection-check.md) | Gömülü özel dosya yükleme talimatı işlenmedi. Elle tehdit değerlendirmesi; bağımsız güvenlik testi veya garanti değil. |

## Görsel inceleme ve düzeltme

Linear [START](examples/linear/start.png) ve [END](examples/linear/end.png), 1672×941. İkisi gerçekten açıldı ve incelendi. Sarı işaret merkezleri (570.83,550.28) → (835.22,549.84), düşey sapma 0.44px. İşaret alanları dışındaki ortalama mutlak RGB farkı 255 ölçeğinde 0.7111. [Ölçüm](examples/linear/measurements.json) incelemeyi destekler; tek başına kalite kanıtı değildir. Sabit kartlar ve kamera, tek işaretin yatay hareketi, sakin üst boşluk ve tüm kartları koruyan mobil contain uygundur. Ara video kareleri üretilmediğinden video morphing testi iddiası yoktur.

Peak Design ilk START kadrajı istenenden büyüktü; END ve iki onarım kumaş dokusunu değiştirdi. Kusur tespit edilerek çekirdeğe ince kumaş/hardware kontrolü ve başarısız çifti ayırma kuralı eklendi. Kusurlu resimler çalışma dizininde saklandı; onaylı örnek olarak paketlenmedi. Kaynak fotoğraflar pakete kopyalanmadı, kaynak bağlantıları verildi. Ürün kimliği bozulursa skill, görsel üretimini başarılı diye sunmaz ve bunu prompt-only başarıya dönüştürmez. Her URL için otomatik kusursuz katalog doğruluğu sözü yoktur.

## Paket ve sınırlar

JSON/YAML, yerel referanslar, arşiv yolları/symlinkler, bilinen anahtar örüntüleri ve dosya hash karşılaştırmaları paketleme sırasında denetlenir. Son sonuç dıştaki `website-to-video-package-validation.json` dosyasına yazılır. Bu denetimler manuel incelemenin veya tam sır taramasının yerine geçmez. Eski Naples/Glacier site düzeltme testleri bu skill'e aitmiş gibi sayılmadı.

Video üretilmedi, oynatım veya gerçek scroll entegrasyonu test edilmedi; zorunlu çıktı video dosyası değildi. Hedef video aracı belirtilmediği için iki-kare desteği varsayılmadı. Örneklerde tek-girdili aracın daha zayıf bitiş kısıtı açıklandı. Kusursuz döngü vaat edilmedi. Claude istemcileri gerçek testten geçmedi. Pranam'a mesaj gönderilmedi.
