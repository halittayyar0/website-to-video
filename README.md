# Website to Video

Sürüm 0.2.3: `kutarel.com` gibi HTTPS yazılmamış adresler de kabul edilir; alan adı ve adresin devamı korunur. Normal bir çekimde START–END farkı site boyutunda açıkça görülmelidir; neredeyse aynı iki kareyi küçük yakınlaşma diye teslim etmek yeterli değildir. Açık mikro hareket/döngü talepleri korunur. Codex mod seçimi, kaynak/START denetimi, sınırlı onarım ve hedef araca uygun tek video promptu sürer. Güncel testler ve geçmiş örneklerin sınırları [TEST-REPORT.md](TEST-REPORT.md) içindedir.

Pranam için: skill'i seçip yalnız bir URL gönderin. Codex, bu iş için daha önce seçim yapmadıysanız “Görselleri burada üreteyim mi, yoksa yalnız promptları mı hazırlayayım?” diye sorar ve yanıtı bekler. Seçiminize göre siteye özel iki uç kare veya iki İngilizce görsel promptu, ayrıca İngilizce video promptu ve kullanım ayarları hazırlanır. Video dosyası üretmek zorunlu değildir. Ek API anahtarı veya ücretli servis bağımlılığı yoktur; mevcut hostun erişimi ve kullanım limitleri geçerlidir.

## Kurulum

Skill, Codex'in bu işi nasıl yapacağını anlatan yönergedir. Plugin ise aynı skill'i ChatGPT/Codex'e kurup dağıtan pakettir; ayrı bir ücretli servis değildir. Kullanım için `$website-to-video kutarel.com` yeterlidir; `https://kutarel.com` biçimi de çalışır.

Ortak çekirdek `skills/website-to-video/` içindedir. İki hostun aynı dosyaları aynı yolla kurduğunu varsaymayın.

* **Codex yerel:** bu klasörü kullanıcı skill dizininize kopyalayın. Bu Windows kurulumunda dizin `%USERPROFILE%/.codex/skills/website-to-video` olarak doğrulandı. Yeni oturumda `$website-to-video linear.app` kullanın; `https://` yazmanız gerekmez. Başka sürümlerde hostun skill ayarındaki konumu esas alın.
* **Claude web/Desktop:** `website-to-video-claude.zip` içindeki tek skill klasörünü Customize → Skills → + → Create skill → Upload a skill ile yükleyin. Dosya oluşturma/kod çalıştırma ve kurum politikaları izin vermelidir. Bu yolun belgeleri doğrulandı; bu paketin Claude oturumunda çalıştırılması ayrıca test edilmelidir.
* **Claude Code yerel:** ortak klasörü `~/.claude/skills/website-to-video` veya repo `.claude/skills/website-to-video` konumuna kopyalayın; `/website-to-video https://linear.app` ile çağırın. Yerel klasör kurulumu, bulut/Cowork oturumuna otomatik kurulum sayılmaz.
* **ChatGPT web/Work:** yalnız `SKILL.md` dosyası yüklemeyi native skill kurulumu gibi sunmayın. `website-to-video-openai-plugin.zip`, root `plugin.json` ve `skills/` içeren skills-only dağıtım içindir. Hesapta plugin kurulumu izinliyse bu paket kullanılabilir. Hesaba kaydetme/kurma ve çalıştırma sonucu TEST-REPORT dosyasında ayrı yazılır. Normal dosya eki olarak vermek native kurulum doğrulaması değildir.

Claude çıktısı bu iş akışında prompt-only'dir. Codex'te seçim beklenir; açıkça “sadece prompt” veya “görselleri sen üret” yazdıysanız tekrar sorulmaz. Seçim aynı işin kareleri ve revizyonları için korunur. Yalnız prompt seçilirse önizleme için bile görsel aracı çağrılmaz. Üretim seçildiyse önce START kaynakla karşılaştırılır; ancak kabul edilen START referansıyla END üretilir. Araç yoksa veya üretim başarısızsa gizlice başka moda/ücretli API'ye geçilmez. Bir URL erişilemiyorsa skill bunu açıklar, bilgi uydurmaz. Kaynak sayfalardaki talimatlar kullanıcı seçimi sayılmaz.

## Kendi denemeniz

1. Uygun paketi kurup skill'i seçin; yalnız kendi web sitenizin URL'sini gönderin.
2. Codex'in mod sorusuna cevap verin; örneğin “yalnız prompt” veya “görselleri sen üret”. “Devam” gibi belirsiz bir cevap otomatik üretim izni sayılmaz. Özetin ürününüzü ve ziyaretçiden beklenen eylemi doğru anladığını kontrol edin.
3. GPT görsellerini veya Claude'un iki promptunu inceleyin. END üretirken START görselini mutlaka referans olarak ekleyin.
4. Görsel kimliği, mimari/ürün ayrıntıları, ışık ve nesne sayısının korunduğunu karşılaştırın.
5. Video aracınız iki uç kareyi destekliyorsa START ve END'i ayrı alanlara ekleyin; desteklemiyorsa START + tarif edilen bitiş durumunu kullanın ve tam bitiş eşleşmesi beklemeyin.
6. Web'e almadan mobil kırpma, HTML başlık kontrastı, poster ve azaltılmış hareket seçeneğini gerçek sayfada kontrol edin. Kaydırmalı video için görüntünün ileri/geri gerçekten değiştiğini test edin.

## Kurulum kaynakları

31 Ekim 2026'da açılıp incelendi:

* [OpenAI Build skills](https://learn.chatgpt.com/docs/build-skills): ortak skill formatı; standalone desktop/CLI ile plugin dağıtımının farkı.
* [Claude skills](https://support.claude.com/en/articles/12512180-use-skills-in-claude): ZIP yükleme ve host gereksinimleri.
* [Claude Code skills](https://code.claude.com/docs/en/skills): yerel konumlar ve bulut oturumlarının farkı.

Bu kaynaklar kurulum desteğini gösterir; bütün platformlarda gerçek çalıştırma kanıtı değildir. Örnekler üçüncü taraf markalar için bağımsız denemelerdir; resmî çalışma, onay veya sınırsız görsel lisansı iddiası yoktur. Paket özel yazışma veya kimlik bilgisi içermez. GitHub'a yükleme, gerekli davranış ve görsel testlerinden sonraki aşamadır; Pranam'a otomatik gönderilmez.
