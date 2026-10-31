# Website to Video, v0.2.0 test raporu

31 Ekim 2026. Yerel Windows/Codex ortamında yapıldı. Belge desteği, dosya kurulumu, elle davranış testi ve başka istemcide gerçek çalıştırma ayrı değerlendirilir.

## Yeni sürümde kontrol edilenler

| Koşu | Gerçek kapsam | Sonuç |
| --- | --- | --- |
| [14 mod senaryosu](tests/mode-forward.json) | Bağımsız ajan güncel skill ve referanslarını okuyup sıradaki yanıtı ve izin verilen adımı üretti. | URL-only soru, açık seçim, seçim devamlılığı/değişimi, belirsiz yanıt, araç yokluğu, enjeksiyon, bakım, iptal, eksik START ve yanıtsız önseçim doğru ayrıldı. Medya, web veya gerçek soru arayüzü çalıştırılmadı; karar düzeyi kanıtıdır. |
| [Yeni Peak prompt-only teslimi](tests/peak-prompts-v2.md) | Bağımsız koşu ürün, ana sayfa ve bağlantılı marka sayfasını gerçekten okudu; iki resmî ürün fotoğrafını açıp inceledi. Önceki örnekleri okumadı. | İki tam İngilizce görsel promptu, video promptu, kaynak kaydı ve mobil/HTML metni planı hazırlandı. Görsel/video çağrısı yok. Tam sayfa render'ı ve gerçek çıktı kırpması doğrulanmadı. |
| [Yeni Naples prompt-only teslimi](tests/naples-prompts-v2.md) | Güncel skill ile URL-only girişin mod sorusu kaydedildi; test düzeneği “Yalnızca promptlar” yanıtını sağladı. Ana sayfa, gerçek bağlantılı ilan ve üç resmî görsel gerçekten incelendi. | Seçilen ilanın kendi şelale fotoğrafı eşleştirildi; başka havuz görseli kullanılmadı. İki tam görsel promptu ve tek video promptu hazırlandı. Mod yanıtı gerçek kullanıcıdan yeniden alınmadı; görüntü/video üretilmedi. |
| [Bağımsız görsel/örnek tekrar incelemesi](tests/quality-review-v2.json) | Linear çiftinin, eski Peak START/END'inin ve resmî kaynak fotoğrafının pikselleri yeniden açıldı; boyutlar PIL ile okundu; üç örneğin video promptları incelendi. | Q1–Q3 kapandı: eski yanlış START'ın geçmişi açık; üç örnekte eksiksiz START-only alternatif var; gerçek boyut ve kadraj farkı yazıldı. Eski Peak çifti reddedilmiş kalır. Bu düzenleme yeni üretim değildir. |
| [Yeni Linear tek-girdi teslimi](tests/linear-prompts-single-input-v2.md) | Gerçek ana sayfa, /plan ve /build okundu; üç resmî varlık görsel incelendi. Kullanıcı aracının yalnız START kabul ettiği bilgisi verildi. | İlk teslimde gereksiz iki-girdi referans bloğu vardı. Skill/şablon dar biçimde düzeltildi, aynı gerçek kaynaklardan teslim adımı yeniden yürütüldü: tam iki görsel promptu ve tek bağımsız START-only video promptu. Yeniden araştırma veya medya üretimi değildir. |
| [Yeni Peak üretim kapısı](tests/peak-generation-v2.json) | Üç gerçek resmî fotoğraf incelendi. Kaynak bağlı START ve iki kaynak bağlı onarım yerleşik görsel aracıyla üretildi, açılıp incelendi. Son START/kaynak ana ajan tarafından da açıldı. | Üç START da ince kumaşı yanlış desenle değiştirdi; 1672×941 çıktı. START reddedildi, END çağrısı yapılmadı, çift başına 2/2 onarımda durdu. Bu davranış kapısının geçmesidir; başarılı katalog görseli veya iki kare üretimi değildir. |
| [Erişim hatası yeniden koşusu](tests/unreachable-v2.json) | Ana ajan `.invalid` adresini web aracıyla yeniden açmayı denedi; gerçek erişim hatası aldı. | Marka analizi veya medya uydurulmadı. Elle negatif yol kontrolü, bağımsız güvenlik testi değil. |
| [Yeni Linear görsel çifti](examples/linear-v2/RESULT.md) | Gerçek güncel kaynaklar, yeni START, gerçek kabul edilmiş START bağlı END ve iki END onarımı. Ana ajan ve [bağımsız görsel inceleme](tests/new-linear-stills-review-v2.json) gerçek pikselleri açtı. | START + ikinci END denemesi aynı sakin soyut konsept için kabul edildi. İlk %2 tasarım hedefi tam sağlanmadı; son video planı gözlenen yaklaşık %3,8–4 yakınlaşmayı açıkça yansıtıyor. Üç ray, tek küre, malzeme ve ışık görsel olarak tutarlı; tam piksel-identik ölçek veya ara video kanıtı yok. Dört çağrı, 2/2 onarım; başka çağrı yok. |

Kayıtların kapsamı: [Peak prompt-only](tests/peak-prompts-v2-execution-scope.json), [Linear tek-girdi](tests/linear-prompts-single-input-v2-execution-scope.json), [son teslim farkı incelemesi](tests/delivery-delta-review-v2.json). Uniform yakınlaşmada bütün görünür boyutların birlikte ölçeklenmesiyle çelişen sabit piksel ölçüsü talimatları da düzeltildi; teslim adımı üçüncü kez yalnız metin düzeyinde tekrarlandı. Resmî kaynak fotoğrafları ve reddedilmiş ürün görselleri dağıtım paketine alınmadı; yerel çalışma kanıtında korundu. Bu rapor kendi başına yayın veya host kurulum başarısı değildir.

Resmî [OpenAI skill formatı](https://learn.chatgpt.com/docs/build-skills), [Claude ZIP kurulumu](https://support.claude.com/en/articles/12512180-use-skills-in-claude) ve [Claude Code konumları](https://code.claude.com/docs/en/skills) yeniden incelendi. Belge desteği gerçek host çalıştırması değildir. [Görsel üretim belgesi](https://developers.openai.com/api/docs/guides/image-generation) de nesiller boyunca tutarlılık ve hassas kompozisyonda sınırlar belirtir. API parametreleri yerleşik aracın argümanları gibi kullanılmadı; ek API/servis eklenmedi.

## v0.1.0'da gerçekte yapılanlar

Aşağıdaki üç sektör koşusu ve yerel kurulum eski sürümün tarihsel kanıtıdır. Yeni mod sorusu/START kapısı o koşularda yürütüldü diye sayılmaz. Güncel durum dış teslim ve yeni test kayıtlarıyla ayrıca doğrulanır.

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

Peak Design ilk START kadrajı istenenden büyüktü; START da kaynak kumaşını bozmuştu. END ve iki onarım bu kusuru gideremedi. Kusur tespit edilerek çekirdeğe ince kumaş/hardware kontrolü ve başarısız çifti ayırma kuralı eklendi. Kusurlu resimler çalışma dizininde saklandı; onaylı örnek olarak paketlenmedi. Kaynak fotoğraflar pakete kopyalanmadı, kaynak bağlantıları verildi. Ürün kimliği bozulursa skill, görsel üretimini başarılı diye sunmaz ve bunu prompt-only başarıya dönüştürmez. Her URL için otomatik kusursuz katalog doğruluğu sözü yoktur.

## Paket ve sınırlar

JSON/YAML, yerel referanslar, arşiv yolları/symlinkler, bilinen anahtar örüntüleri ve dosya hash karşılaştırmaları paketleme sırasında denetlenir. Son sonuç dıştaki `website-to-video-package-validation.json` dosyasına yazılır. Bu denetimler manuel incelemenin veya tam sır taramasının yerine geçmez. Eski Naples/Glacier site düzeltme testleri bu skill'e aitmiş gibi sayılmadı.

Video üretilmedi, oynatım veya gerçek scroll entegrasyonu test edilmedi; zorunlu çıktı video dosyası değildi. Hedef video aracı belirtilmediği için iki-kare desteği varsayılmadı. Örneklerde tek-girdili aracın daha zayıf bitiş kısıtı açıklandı. Kusursuz döngü vaat edilmedi. Claude istemcileri gerçek testten geçmedi. Pranam'a mesaj gönderilmedi.
