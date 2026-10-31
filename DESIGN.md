# Tasarım ve çalışma planı

## v0.2.5: yaratıcı brief zorunlu değil

Sadece site adresi veren kullanıcı, belirtilmemiş yaratıcı kararları ajana bırakmış sayılır. Araştırmadan sonra tek uygulanabilir yön seçilir ve iş yürütülür; sahne/stil/kamera listesi veya rutin konsept onayı istenmez. Önceki beş saniye, 16:9 veya ürün eylemi örnekleri evrensel şablon değildir. Kullanıcı açık gereksinim verirse o gereksinim korunur. Mod sorusu yalnız çıktı tercihidir; yaratıcılık onayı değildir. Bu serbestlik ürün hakkında gerçek uydurma veya yetkisiz harcama/yayın/mesaj hakkı vermez.

## v0.2.4: ürüne özel eylem, kamera farkından ayrı

Kullanıcı v0.2.3'teki daha büyük KUTAREL zoomunu da reddetti: kadraj farkı ile sahne eylemi aynı şey değildir. Yeni hedef yalnız daha fazla zoom değildir. Sahne sitenin gerçek ürünü, kullanım amacı, marka dili ve ziyaretçi eylemine göre seçilir; sabit bir hareket reçetesi uygulanmaz. START/ara eylem/END planlanmadan statik katalog başlangıcı üretilmez. Kamera sabitlenince de sahne eylemi anlaşılmalıdır. Gerçek ürün özelliği ile önerilmiş editorial staging ayrılır; fark yaratmak için gizli yüzey, üretim yöntemi veya malzeme yeteneği uydurulmaz. Açık kamera hareketi/mikro hareket/döngü brief'i geçerlidir. Bu bakım turunda kullanıcı yeni medya istemedi; yalnız skill davranışı ve mevcut dağıtımları değiştirilir.

## v0.2.3: adres girişi ve okunur görsel ilerleme

KUTAREL'in gerçek ilk çiftinde yaklaşık %3,9 yakınlaşma vardı; kullanıcı iki kareyi aynı buldu. Önceki %2–4 varsayılanı ve yalnız küçük değişim isteyen kabul ölçütü bu teslimi gereğinden zayıf bıraktı. Normal, döngüsüz bir çekimde site boyutunda açık görsel ilerleme aranır; bunun için keyfi bir evrensel yüzde şartı yoktur. Kullanıcının açık mikro hareket veya tam çevrim isteği korunur. Kaynakta görünmeyen ürün yüzeyleri ya da doku ayrıntıları fark yaratmak için uydurulamaz.

URL girdisi şemasız alan adı/yol/sorguyu da kapsar; yalnız eksik web şeması eklenir, alan adı tahmin edilmez. Skill yerel çalışma yönergesidir; mevcut private plugin aynı yönergeyi dağıtan pakettir. Bu düzeltme yeni servis ya da site gerektirmez. Güncel davranış denemeleri eski üç sektör testlerinden ayrı raporlanır.

Hedef: URL dışında zorunlu girdi olmadan, web'e gömülmeye uygun tek sahnenin başlangıç ve bitiş görselleri ve video promptu. Genel reklam üreticisi veya web sitesi dağıtım aracı değil.

Seçim: ortak SKILL.md çekirdeği + Claude skill ZIP + OpenAI skills-only plugin. Kullanıcının makul kararlar alıp gereksiz soru sormama isteği doğrultusunda uygulama kararıdır. Ayrı sunucu/API daha fazla bağımlılık eklediği; yalnız Custom GPT yönergesi native skill kurulumunu karşılamadığı için seçilmedi.

Sıra: gerçek host formatlarını ve kaynak siteleri incele; çekirdeği ve referansları yaz; gerçek URL'lerle uçtan uca davranışları dene; bir GPT görsel çiftini START referanslı END ile üret ve incele; prompt-only ve erişim hatasını değerlendir; kusurları düzeltip yeniden dene; paketleri doğrula; geçer kanıtından sonra private GitHub yüklemesi; kurulum durumunu ve sınırlamaları teslim et. Video üretimi zorunlu değil ve üretilmeyen video test edilmiş sayılmaz.

Yayın kapısı: üç farklı sektörün URL-only örnekleri, görsel araçlı ve prompt-only yollar, erişilemeyen site, görsel tutarlılık ve hareket uygulanabilirliği kanıtları hazır olmadan GitHub'a yükleme yapılmaz. Claude çalıştırma erişimi yoksa belgelenmiş destek ile gerçek çalıştırma ayrı raporlanır. Gizli veri, önceki müşteri yazışmaları ve yetki dosyaları pakete alınmaz.

## v0.2.2: açık çekim talebini koruma

Bağımsız A denemesinde kullanıcı360 derece/önden arkaya çekim istedi. Mevcut skill özgün çekimi engelli diye doğru etiketlerken yine de tam bir önden%2 yakınlaşma teslimi hazırladı. Bu, etiket dürüstlüğünü sağlar ama istenen işi karşılamaz. Kök çelişki: tam iki prompt teslim şartının, kaynak/çekim imkânsızlığında durma şartına önceliği belirsizdi; küçük hareket kuralı da varsayılan yerine mutlak yazılmıştı.

Dar düzeltme: iki uçlu tam teslim yalnız çözümlenmiş uygulanabilir çekim içindir. Açık hareket, son açı, süre, oran ve sadakat korunur; maddi çelişki veya eksik arka görünümde ilgili END/video bekler. Kullanıcı önceden alternatif seçimini devretmişse izin verilen alternatif uygulanır. Döngüde tam çevrim ile END'in rolü ayrı açıklanır; geri oynatma tek yönlü fiziksel hareket için evrensel çözüm değildir.

Test kapsamı bu metin/karar değişikliğidir: donmuş başarısız baz yanıtı, güncel skill ile bağımsız yeniden kullanım ve olumlu/olumsuz karşı örnekler. Eski gerçek kaynak araştırması ve görsel çiftleri tarihsel kanıt olarak korunur; yeni görüntü/video üretimi veya bütün hostlarda yürütme gibi sayılmaz.

## v0.2.0 iyileştirmesi

Kullanıcının yeni tercihi: Codex her yeni işte açık seçim yoksa görselleri üretmek ile yalnız prompt hazırlamak arasında bir kez sorar. URL tek proje girdisi olmaya devam eder; bu soru ek yaratıcı brief değildir. Aynı işte revizyon ve onarımlar seçimi korur. Yanıtsız soru veya araç mevcudiyeti üretim seçimi sayılmaz. Bakım talepleri normal üretim işi değildir.

Gözlenen kusurlara yönelik değişiklikler: START kaynak kimliğini geçmeden END çağrısı yok; onarım bütçesi çift başına iki ek çağrı; reddedilmiş END yeni süreklilik referansı olamaz. Tek başlangıç görseli kabul eden hedef için END ekine dayanmayan tam video promptu gerekir. Gerçek boyut ve kırpma hedefi, ölçülmüş sonuçtan ayrı raporlanır. Bu kurallar mevcut başarısız ürün örneğini başarılı saymak için kullanılmaz.

Doğrulama sırası: bağımsız karar senaryoları; gerçek kaynaklardan yeni prompt-only koşuları; gerçek araçla yeni START/END kalite kapısı koşusu; eski Linear ve başarısız ürün piksellerinin bağımsız incelemesi; kaynak/paket/yerel kurulum karşılaştırması; mevcut private depo ve plugin'e güncelleme; sunucudan geri okuma. Modelin her ürünü kusursuz yeniden çizeceği iddiası yoktur. Başarı ölçütü, talep edilen akışın kanıtla uygulanması ve uygun olmayan çıktının açıkça ayrılmasıdır.
