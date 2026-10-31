# Tasarım ve çalışma planı

Hedef: URL dışında zorunlu girdi olmadan, web'e gömülmeye uygun tek sahnenin başlangıç ve bitiş görselleri ve video promptu. Genel reklam üreticisi veya web sitesi dağıtım aracı değil.

Seçim: ortak SKILL.md çekirdeği + Claude skill ZIP + OpenAI skills-only plugin. Kullanıcının makul kararlar alıp gereksiz soru sormama isteği doğrultusunda uygulama kararıdır. Ayrı sunucu/API daha fazla bağımlılık eklediği; yalnız Custom GPT yönergesi native skill kurulumunu karşılamadığı için seçilmedi.

Sıra: gerçek host formatlarını ve kaynak siteleri incele; çekirdeği ve referansları yaz; gerçek URL'lerle uçtan uca davranışları dene; bir GPT görsel çiftini START referanslı END ile üret ve incele; prompt-only ve erişim hatasını değerlendir; kusurları düzeltip yeniden dene; paketleri doğrula; geçer kanıtından sonra private GitHub yüklemesi; kurulum durumunu ve sınırlamaları teslim et. Video üretimi zorunlu değil ve üretilmeyen video test edilmiş sayılmaz.

Yayın kapısı: üç farklı sektörün URL-only örnekleri, görsel araçlı ve prompt-only yollar, erişilemeyen site, görsel tutarlılık ve hareket uygulanabilirliği kanıtları hazır olmadan GitHub'a yükleme yapılmaz. Claude çalıştırma erişimi yoksa belgelenmiş destek ile gerçek çalıştırma ayrı raporlanır. Gizli veri, önceki müşteri yazışmaları ve yetki dosyaları pakete alınmaz.
