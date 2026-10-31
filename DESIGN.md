# Tasarım ve çalışma planı

Hedef: URL dışında zorunlu girdi olmadan, web'e gömülmeye uygun tek sahnenin başlangıç ve bitiş görselleri ve video promptu. Genel reklam üreticisi veya web sitesi dağıtım aracı değil.

Seçim: ortak SKILL.md çekirdeği + Claude skill ZIP + OpenAI skills-only plugin. Kullanıcının makul kararlar alıp gereksiz soru sormama isteği doğrultusunda uygulama kararıdır. Ayrı sunucu/API daha fazla bağımlılık eklediği; yalnız Custom GPT yönergesi native skill kurulumunu karşılamadığı için seçilmedi.

Sıra: gerçek host formatlarını ve kaynak siteleri incele; çekirdeği ve referansları yaz; gerçek URL'lerle uçtan uca davranışları dene; bir GPT görsel çiftini START referanslı END ile üret ve incele; prompt-only ve erişim hatasını değerlendir; kusurları düzeltip yeniden dene; paketleri doğrula; geçer kanıtından sonra private GitHub yüklemesi; kurulum durumunu ve sınırlamaları teslim et. Video üretimi zorunlu değil ve üretilmeyen video test edilmiş sayılmaz.

Yayın kapısı: üç farklı sektörün URL-only örnekleri, görsel araçlı ve prompt-only yollar, erişilemeyen site, görsel tutarlılık ve hareket uygulanabilirliği kanıtları hazır olmadan GitHub'a yükleme yapılmaz. Claude çalıştırma erişimi yoksa belgelenmiş destek ile gerçek çalıştırma ayrı raporlanır. Gizli veri, önceki müşteri yazışmaları ve yetki dosyaları pakete alınmaz.

## v0.2.0 iyileştirmesi

Kullanıcının yeni tercihi: Codex her yeni işte açık seçim yoksa görselleri üretmek ile yalnız prompt hazırlamak arasında bir kez sorar. URL tek proje girdisi olmaya devam eder; bu soru ek yaratıcı brief değildir. Aynı işte revizyon ve onarımlar seçimi korur. Yanıtsız soru veya araç mevcudiyeti üretim seçimi sayılmaz. Bakım talepleri normal üretim işi değildir.

Gözlenen kusurlara yönelik değişiklikler: START kaynak kimliğini geçmeden END çağrısı yok; onarım bütçesi çift başına iki ek çağrı; reddedilmiş END yeni süreklilik referansı olamaz. Tek başlangıç görseli kabul eden hedef için END ekine dayanmayan tam video promptu gerekir. Gerçek boyut ve kırpma hedefi, ölçülmüş sonuçtan ayrı raporlanır. Bu kurallar mevcut başarısız ürün örneğini başarılı saymak için kullanılmaz.

Doğrulama sırası: bağımsız karar senaryoları; gerçek kaynaklardan yeni prompt-only koşuları; gerçek araçla yeni START/END kalite kapısı koşusu; eski Linear ve başarısız ürün piksellerinin bağımsız incelemesi; kaynak/paket/yerel kurulum karşılaştırması; mevcut private depo ve plugin'e güncelleme; sunucudan geri okuma. Modelin her ürünü kusursuz yeniden çizeceği iddiası yoktur. Başarı ölçütü, talep edilen akışın kanıtla uygulanması ve uygun olmayan çıktının açıkça ayrılmasıdır.
