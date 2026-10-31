# Website to Video, v0.2.6 test raporu

31 Ekim 2026. Yerel Windows/Codex ortamında yapıldı. Belge desteği, dosya kurulumu, elle davranış testi ve başka istemcide gerçek çalıştırma ayrı değerlendirilir.

## v0.2.6: video promptu sohbet içinde

Dar teslim biçimi düzeltmesi: çözümlenmiş çekimin tam İngilizce video promptu, hem görsel üretimi hem prompt-only modunda, son sohbet yanıtında tek fenced text bloğunda zorunludur. Dosya/ZIP bağlantısı, özet, kısaltılmış metin, placeholder veya sonradan sunma teklifi yeterli değildir. Ek dosya varsa inline tam metinle aynı olmalıdır. Gerçekten çözümlenmemiş işin bekletilmesi korunur; blok doldurmak için uydurma üretim yapılmaz.

Çekirdek, sonuç şablonu ve değerlendirme ölçütü birlikte düzenlendi; kaynak metin incelemesi, skill sözdizimi ve paket/yerel/remote dosya eşliği kontrol edilir. Bu küçük biçim değişikliğinde yeni model davranış koşusu, site araştırması veya medya üretimi yapılmadı. Önceki davranış/görsel testleri tarihsel kapsamıyla korunur.

## v0.2.5: yaratıcı karar sahipliği ve genel dağıtım

Kullanıcı yaratıcı brief vermediğinde yalnız URL yeterlidir. Ajan siteyi/ürünü araştırır; konuyu, sahneyi, eylemi, stili, kamerayı, ritmi, süreyi, oranı ve kompozisyonu seçer, olağan bir konsept onayı için durmaz. Açık kullanıcı isteği önceliklidir. Örnek sahneler veya beş saniye/16:9 gibi önceki öneriler evrensel reçete değildir. Çıktı modu sorusu ayrı bir teslim tercihidir; yaratıcı brief veya tekrar eden onay kapısı olmaz. Kaynak doğruluğu, hareket tutarlılığı ve kanıt dürüstlüğü kalite şartı olarak kalır.

Bağımsız [dört gerçek karar/plan yanıtı](tests/v025-forward/responses.md) ve [inceleme/hash kaydı](tests/v025-forward/review.json) geçti: yalnız URL'de tek teslim tercihi sorusu ve sıfır yaratıcı brief sorusu; fırın fixture'ında marka/ürüne dayalı sahne seçimi; yazılım fixture'ında açıkça temsili, gerçek arayüz iddiası taşımayan koordinasyon sahnesi; açık 9:16/8 saniye/sabit kamera/insansız çeşme isteğinin korunması. Süre/oran önceki önerilere zorlanmadı, konsept onayında durulmadı. Beş değerlendirilen dosya hash'i güncel kaynakla karşılaştırılır. Bunlar canlı kaynak araştırması veya medya üretimi değil, sağlanan öncüllerle davranış planlarıdır.

Bu bakımda yeni medya veya yeni canlı site analizi yapılmadı. Güncel davranış denemeleri ve yerel kurulum/yayın kanıtları ayrı kaydedilir. README genel kullanıcıya göre düzenlendi. GitHub'ın herkese açılması ayrıca gerçek görünürlük ve anonim erişimle doğrulanır; eski private yayın kayıtları geçmiş durumdur.

## v0.2.4: siteye ve ürüne özel gerçek sahne eylemi

Kullanıcı, v0.2.3 KUTAREL tam ürün → detay çiftini de hareket ihtiyacına uygun bulmadı. Daha büyük yakınlaşma, nesnenin/sahnenin eylemsiz kalmasını çözmez. Önceki görsel kadraj farkı kabulü bu yeni hareket talebini geçtiği anlamına gelmez. [Gerçek başarısız örnek kaydı](tests/v024-baseline/static-zoom.json).

Düzeltme: plan incelenen site/ürün kanıtından başlar; eylemin neden bu ürüne ve sayfaya uyduğu açıklanır. Hareket eden unsur, START/ara/END durumları ve zamanlama, kameranın destek rolünden ayrı yazılır. Normal hareket isteğinde kamerayı zihnen sabitleyince hâlâ sahne eylemi kalmalıdır. Her büyüklükte yalnız statik kırpma/zoom varsayılan çözüm olarak reddedilir. Sabit dönüş/kumaş/rastgele el-model şablonu uygulanmaz. Kimlik ve yapı sabit tutulurken gerekli poz/konum/uygun yumuşak hareketin değişmesine izin verilir; tüm silueti dondurmak eylemi iptal edemez. Eksik gerçek görünüm/özellik uydurulmaz. Açık camera-only, mikro hareket veya çevrim talebi korunur.

İlk bağımsız [dört yanıt](tests/v024-baseline/first-next-responses.md), çanta için doğrulanmış fermuar açılışı, kafe için kaynakta görülen dökme eylemi ve açık camera-only istisnasını uygun planladı. Ancak KUTAREL'de yalnız statik kaynak bulunduğu için kullanıcıdan zorunlu hareket kaydı istedi. [Ana ajan değerlendirmesi](tests/v024-baseline/first-candidate-assessment.json) bu kısmı gereksiz engel olarak reddetti; bağımsız ilk incelemenin genel PASS etiketi son kabul sayılmadı. Statik kaynak, editoryal hareket tasarlamayı tek başına engellemez; gerçek özellik/demonstrasyon kanıtı ile açıklanmış görsel sahneleme ayrıldı. Kaynakta olmayan arka yüz veya kesin malzeme/performans iddiaları için kanıt şartı korunur.

Güncel adayla [KUTAREL yeniden yanıtı](tests/v024-forward/kutarel-rerun.md) ve [inceleme/hash kaydı](tests/v024-forward/rerun-review.json) geçti: örnek marka öncüllerine bağlı sakin, önden masa üstü giysi düzenleme eylemi; ellerin manşetleri dışa kaydırıp çekildiği gerçek START/ara/END durumları. Bu plan sabit kamerada da eylem taşır, mevcut eski katalog START'ını zorlamaz; gerçek kumaş performansı iddiası ve kullanıcıdan zorunlu hareket kaydı yoktur. Beş değerlendirilen çekirdek/referans dosyasının hash'i yayın adayına eşleştirilir. İlk üç diğer dalın uygun planları ve hatalı ilk KUTAREL engeli tarihsel kayıt olarak korunur.

Bu testler sağlanan fixture'lardan üretilmiş gerçek karar/metin yanıtlarıdır; canlı site araştırması, tam üç-prompt teslimi veya medya üretimi değildir. Eski gerçek KUTAREL iki görseli açılıp hareket ihtiyacına uymadığı belirlendi. Bu sürüm skill bakımıdır; yeni KUTAREL kareleri veya video üretilmedi. Yeni sahnenin temas, kimlik, kırpma ve ara hareket başarısı üretilmiş görüntü/video olmadan doğrulanamaz.

## v0.2.3: şemasız adres ve fark edilebilir uç kareler

Kullanıcının gerçek KUTAREL ilk çiftine verdiği geri bildirim, yaklaşık %3,9 global yakınlaşmanın bu işte yetersiz olduğunu gösterdi. [Başarısız başlangıç kaydı](tests/v023-baseline/kutarel-motion-failure.json) eski çıktıyı başarı örneği saymaz. Kök neden, varsayılan %2–4 küçük yakınlaşma ile görsel ilerleme kontrolü eksikliğidir.

Yeni çekirdek şemasız web adresini HTTPS ile tamamlar; alan adı/yol/sorgu/portu korur. Normal çekimde gerçek ekranda anlaşılır START → END ilerlemesi aranır; açık mikro hareket ve tam çevrim talepleri korunur. KUTAREL revizyonunda kabul edilmiş START aynı kaldı ve gerçek START referanslı yeni END üretildi. Bu revizyon yeni kaynak/mağaza durumu araştırması veya site değişikliği değildir.

Bağımsız [altı gerçek metin yanıtı](tests/v023-forward/responses.md) ve [değerlendirme](tests/v023-forward/review.json): yeni şemasız URL'de tek mod sorusu; mevcut prompt-only seçiminde port/yol/sorgu/fragment korunması; açık HTTP ve mikro hareketin korunması; doğrulanmış tüm-yüz fixture'ında tam 360° çevrim; hatalı alan adında sessiz başka domaine geçmeme; web dışı şemayı açmama. Altı karar/metin senaryosu geçti. Bunlar canlı web veya altı gerçek host çalıştırması değildir.

Gerçek yerel piksellerin bağımsız incelemesi, ilk yeni END'in belirgin farkını geçti fakat kaynağın göstermediği rib yaka dokusunu reddetti. Gerçek START bağlı son onarım sonrası [takip incelemesi](tests/v023-forward/repair-follow-up.json), bu dokunun kalktığını ve açık tam ürün → detay ilerlemesini doğruladı. Genel süreklilik, kaynak türevli dijital mockup konsepti düzeyinde geçti; birebir yaka/işaret geometrisi doğrulanmadı. İki kare 1672×941. Mobil `contain`, medya dışında HTML metni gerekir; merkezden portre kırpma onaylanmaz. Bu revizyonda iki yeni END çağrısı yapıldı; reddedilmiş END yeni referans yapılmadı, çift başına iki ek onarım sınırında duruldu.

Eski üç sektörün gerçek kaynak ve medya testleri aşağıda tarihsel kanıt olarak kalır; güncel sürümde yeniden çalıştırılmış sayılmaz. Video dosyası ve ara kareler üretilmedi; Claude çalıştırması istenmedi ve yapılmadı. Yeni paket/dosya/yerel kurulum ve uzaktan kaynak geri okuması dış teslim kayıtlarında ayrı doğrulanır.

## v0.2.2: açık çekim talebi ve çözümlenmemiş gereksinimler

[Donmuş baz yanıtlar ve inceleme](tests/v022-baseline/review.json), v0.2.1'e aittir; v022 dosya/koşu adları iyileştirme kampanyasını belirtir. [Kaynak sürüm kaydı](tests/v022-baseline/provenance.json) bunu sabitler. A yanıtı,360 derece/önden arkaya çelişkisini ve eksik arka görünümü doğru bulduğu hâlde istenmemiş tam bir önden yakınlaşma teslimi yaptı. Şeffaf alternatif etiketi, özgün kapsamın karşılandığı anlamına gelmez.

Dar düzeltme: tam iki uç teslimi çözümlenmiş uygulanabilir çekime bağlandı; varsayılan küçük hareket açık talebin yerine geçmez. Net son açı, dönüş hızı, eksik gerçek ürün görünümü ve döngünün tam çevrimi kontrol edilir. Gerekli END/video bekletilir; kullanıcı alternatif seçimini devretmişse o yetki korunur.

[Yeni bağımsız koşu](tests/v022-rerun/evaluation.json), önceki yanıtları okumadan güncel skill ve referansları kullanıp altı gerçek metin yanıtı yazdı. Ana ajan yanıtları okudu ve değerlendirilen beş dosyanın SHA256 değerlerini güncel adayla eşleştirdi. Bunlar mevcut yerel kaynaklardan test fixture'larıdır; yeni canlı araştırma, yeni görsel/video üretimi veya başka hostta yürütme değildir. Resmî kaynak fotoğrafları ve reddedilmiş üretim denemeleri bu pakete eklenmedi; ham kaynak yolları yalnız yerel test girdilerini tanımlar.

| Vaka | Gözlenen sonuç ve kanıt |
|---|---|
| [A — çelişen gerçek ürün dönüşü](tests/v022-rerun/A-response.md) |360 derece sonunda ön poz, arka END için180 derece ve72 derece/saniye hesaplandı. Tek gerekli açı kararı ve eksik arka/yan kaynaklar istendi; istenmemiş tam alternatif yazılmadı. Özgün çekim **beklemede**. |
| [B — mobil kırpma / HTML metni](tests/v022-rerun/B-response.md) | İki bağımsız İngilizce uç promptu ve çift-girdili video promptu; dar ortak merkez alanı ve mobilde üstte HTML metni. Yeni üretim/kırpma/kontrast **doğrulanmadı**. |
| [C — farklı açı ve kusursuz döngü](tests/v022-rerun/C-response.md) | END habersizce orta kareye çevrilmedi. Tek geçiş ile başlangıç durumuna dönen tam çevrim arasındaki karar istendi; END/video **beklemede**. |
| [D — önceden izin verilmiş alternatif](tests/v022-rerun/D-response.md) | İzin verilmiş önden%2 yakınlaşma9:16 korunarak tam iki uç ve yalnız START girdili tek video promptuyla hazırlandı. Gerçek kumaş/logo sadakati **doğrulanmadı**. |
| [E — uygulanabilir tam dönüş](tests/v022-rerun/E-response.md) | Özgün kurgu küpte beş saniyede360 derece korundu; hareket küçük yakınlaşmaya dönüştürülmedi. Altı sabit yüz, çeyrek tur zamanları ve ön/ön uçlar tarif edildi. Ara video geometrisi **doğrulanmadı**. |
| [F — doğrulanmamış gerçek otel imkânı](tests/v022-rerun/F-response.md) | Kaynakta olmayan masa/kahvaltı “doğrulanmış” diye yazılmadı. Aynı oda kaynağı ve imkân doğrulaması eksik; gerçek çekim/etiket **beklemede**. Kurgu alternatifi seçilmiş gibi genişletilmedi. |

Altı vakada karar/metin düzeyi davranış uygun bulundu: üç tamamlanmış prompt-only teslim, üç doğru bekletilmiş iş. Bu, altı videonun veya altı görsel çiftinin başarılı üretimi değildir. İnceleme kalan görüntü/video/host kanıtlarını özellikle açık bırakır; evrensel kusursuzluk iddiası yoktur. Mevcut mod seçimi, START-referanslı END ve çift başına iki onarım korunur. Aşağıdaki gerçek kaynak/görsel koşuları önceki sürümlerin kanıtıdır;0.2.2'de yeniden üretilmiş sayılmaz.

## v0.2.0 / v0.2.1'de kontrol edilenler

Metadata yama sürümü 0.2.1: aşağıda sınanan skill davranışı aynı kalır; sunucudaki önceki yazar kimliği korunur. Paylaşılabilir paket yazar iletişim e-postası içermez. Metadata geri okuması dış teslim kanıtında ayrıca doğrulanır.

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
