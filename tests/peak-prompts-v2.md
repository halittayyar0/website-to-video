# Peak Design Everyday Backpack — yalnızca promptlar

Mod: **Prompts only**. Görsel veya video üretilmedi. İnceleme tarihi: 31 Ekim 2026.

Peak Design bu ürünü günlük kullanım ve fotoğraf ekipmanı taşıma için sunuyor; incelenen ürün sayfasında Black, 20L ve 30L seçenekleri bulunuyor. Erişilen bölgesel görünümde ürün stok dışı ve işlem çağrısı “notify me”; film stok veya teslimat iddiası taşımamalı. [Ürün sayfası](https://www.peakdesign.com/eu/products/everyday-backpack)

Önerim, ürün galerisinden sonra ve özellik anlatımından önce kullanılacak, tek çantayı önden gösteren sessiz beş saniyelik bir ürün filmi. Bu yaratıcı tercih, günlük taşıma/fotoğraf kullanıcısının ürünün şeklini ve yüzeyini değerlendirmesine yardımcı olur; çantanın açılması veya bir özellik gösterisi vaat etmez. Beyaz zemin, siyah dokuma yüzey ve kontrollü yakınlaşma incelenen resmi ürün fotoğraflarına dayanır; yerleşim, süre ve hareket aşağıdaki tasarım kararlarıdır.

## Kaynak kaydı

| Kaynak | Gerçekte incelenen / sınır |
|---|---|
| [Ürün URL'si](https://www.peakdesign.com/products/everyday-backpack) → [EU görünümü](https://www.peakdesign.com/eu/products/everyday-backpack) | Metin, seçenekler, CTA ve resmi görsel bağlantıları okundu. Günlük/fotoğraf taşıma, MagLatch ve yan erişim ürün metninde var; film bunları hareketle canlandırmıyor. Bölge ve stok durumu değişebilir. |
| [Ana sayfa](https://www.peakdesign.com/) | Ürün aileleri, ürün odaklı dil ve marka gezinmesi metin olarak incelendi. Tam sayfa render'ı, tipografi, gerçek sayfa renkleri ve responsive düzen görsel olarak doğrulanmadı. |
| [Our Mission](https://www.peakdesign.com/global/pages/mission) | Ana sayfadan izlenen bağlantı; ürün tasarımını ve fotoğraf ekipmanı taşıma kökenini açıklayan marka bağlamı okundu. Film için yeni ürün iddiası türetilmedi. |
| [Resmi turntable 01](https://cdn.shopify.com/s/files/1/2986/1172/files/1_BEDB-20-BK-2.jpg?v=1682534543) | **Görsel olarak açılıp incelendi.** Tek siyah çanta önden, beyaz fonda; dokuma yüzey, geniş üst kapak, orta mandal, üst sap, iki yandaki fermuar hatları ve alttaki kayış uçları görülüyor. Ürün kimliği için birincil referans bu dosya. |
| [Resmi Black 20L galeri fotoğrafı](https://cdn.shopify.com/s/files/1/2986/1172/files/everyday-backpack-black-20-1.jpg?crop=center&height=1024&v=1762275581&width=1024) | **Görsel olarak açılıp incelendi.** Aynı ürün ailesinin ön görünümü ve beyaz ürün fotoğrafı dili teyit edildi. Ayrı çekimdeki doku/ışık farklarını birleştirerek yeni ürün geometrisi yapılmayacak. |

## Süreklilik kilidi

Tek ürün: resmi turntable 01'deki siyah 20L Everyday Backpack. Kapak, gövde dış çizgisi, merkez mandalı, sap, fermuarlar, dikişler, dokuma ve kayışların konumu referansla aynı kalmalı. Ürün önden dik, yatay merkezde; beyaz kesintisiz stüdyo arka planı ve zemine temas gölgesi sabit. Işık üst soldan yumuşak ve nötr; kamera tam karşıda, perspektif ve odak uzaklığı sabit. Tek değişim, görüntü düzleminde merkezden %2 büyüme; orbit, parallax, açılma veya yeni yüzey gösterimi yok. İstenen başlangıç yerleşimi yaklaşık x=%37–63, y=%18–82; END aynı merkez çevresinde %2 büyür. Bunlar üretilecek görsellerin ölçülmüş sınırları değil, kompozisyon hedefleridir.

## START — İngilizce görsel promptu

Önce aşağıdaki resmi turntable görselini indirip üretim aracına **source identity reference** olarak ekleyin. Bu adım burada yapılmış bir görsel üretimi değildir.

```text
Create the START still for a quiet five-second embedded product film on Peak Design's Everyday Backpack product page, placed after the product gallery and before the feature section. Output a 16:9 landscape master, preferably 1920 x 1080 if the chosen tool supports it. This is a faithful product presentation, not a lifestyle advertisement.

Attach this official photograph as the source identity reference: https://cdn.shopify.com/s/files/1/2986/1172/files/1_BEDB-20-BK-2.jpg?v=1682534543 . It shows the black 20L Everyday Backpack directly from the front. Use the attached photograph, not a text-only guess, to preserve the exact visible silhouette, broad tapered top flap, central latch and fastening details, top carry handle, two side zipper paths, seams, fine woven fabric texture, side folds and visible strap ends. Do not blend it with other product variants. Retain visible original product details; do not invent, enlarge or redraw branding. Do not invent unreadable lettering.

Reframe this one upright, closed backpack on a seamless neutral white studio background with its natural grounded contact shadow. Preserve the reference's straight-on product view without revealing a side, back or interior. Keep the entire backpack and its strap tips visible, centered horizontally and vertically; target its complete bounding box at roughly x=37–63% and y=18–82% of the frame. Do not crop the handle or base. This narrow central composition is intentional for later mobile framing, subject to checking the actual output.

Use a fixed front-facing camera with a natural long-lens product-photography perspective, approximately an 85 mm full-frame look, without changing the reference geometry. Soft neutral illumination comes from upper left; fixed exposure and white balance, gentle surface highlights, fine textile detail and a soft contact shadow. Keep the surface matte and black rather than shiny or metallic. No horizon line, props, pedestal, person, camera equipment, scenery, graphic decoration or extra object. The white left region x=5–28%, y=20–75% must remain quiet for optional live HTML copy on desktop. Generate no overlay text, slogan, price, badge, watermark or added logo. The still shows no motion and no product feature demonstration.

This is the accepted-START candidate only. Compare its construction and fine details against the attached official source before using it as the END reference; reject a materially inaccurate product rendition.
```

## END — İngilizce görsel promptu

```text
Use the generated START image as the primary image reference. Attach the actual accepted START still as the edit target and primary continuity anchor. Attach the official source photograph only as a secondary product-identity check: https://cdn.shopify.com/s/files/1/2986/1172/files/1_BEDB-20-BK-2.jpg?v=1682534543 . Do not independently recreate the backpack from this text. If START is not faithful to the official photograph, stop and repair START before attempting this END.

Create the END still of the same quiet five-second embedded product film for Peak Design's Everyday Backpack product page. Keep the exact same 16:9 canvas and output dimensions as START. The scene contains exactly one upright, closed black 20L Everyday Backpack, directly front-facing, centered on a seamless neutral white studio background with a grounded soft contact shadow. Preserve START's precise silhouette, broad tapered top flap, central latch and fastening details, top handle, paired side zipper paths, seams, fine woven fabric pattern, side folds, strap ends, original visible product marks and every material boundary. Do not add, remove or reinterpret construction or branding.

The only change is a small image-plane push-in: enlarge the entire photographed scene by 2% about the exact frame center, equivalent to a 1.02 scale from START. Preserve the aspect ratio and relative positions of every detail. START's intended product bounds are approximately x=37–63%, y=18–82%; the slightly larger END must still show the complete handle, bag and strap tips with ample margins. The view angle and perspective stay fixed; no camera orbit, lateral move, tilt, lens change, parallax or newly visible surfaces. The backpack does not rotate, open, breathe or move; straps, flap and latch do not animate.

Keep the same upper-left soft neutral lighting, matte black textile appearance, white background, shadow direction, exposure, white balance, focus and depth of field. No lighting transition or moving highlight. Maintain quiet desktop copy space at x=5–28%, y=20–75%. No extra object, person, prop, scenery, text overlay, price, badge, watermark or new logo. This is a feasible later instant in the same shot, not a second composition, dissolve or alternate product photograph. Preserve tiny seam and textile details rather than smoothing or redrawing them.
```

## VIDEO PROMPT — İngilizce

Hedef video aracı belirtilmedi. Aşağıdaki blok, **iki uç görseli girdi olarak kabul ettiği doğrulanan** bir araç içindir; herhangi bir sağlayıcı parametresi veya uç kare desteği varsayılmıyor. Tek görsel kabul eden araçta yalnız START eklenmeli ve bitişin merkezden %2 büyüme olduğu metinle tarif edilmeli; END o durumda zorlanan son kare değildir. Seçilmiş bir araç olmadığı için ayrıca varsayımsal bir tek-girdi promptu çoğaltılmadı.

```text
Create a silent five-second product film for the Peak Design Everyday Backpack product page, intended as an embedded insert after the product gallery and before the feature section. Use the supplied START image as the initial visual input and the supplied END image as the final visual target, only through your tool's verified supported endpoint-input mechanism. START and END depict the same single closed black 20L Everyday Backpack, upright and exactly front-facing on a seamless neutral white studio background with a soft grounded contact shadow. Keep a 16:9 landscape frame at the input aspect ratio.

The backpack is the entire subject. Preserve its exact photographed identity: silhouette, broad tapered top flap, central latch and fastening details, top carry handle, two side zipper paths, seams, fine woven textile texture, side folds, original visible product marks and strap ends. Its intended START framing is centered, with the full subject approximately within x=37–63% and y=18–82%. END is the same image-plane view enlarged by just 2% around the frame center. Keep every part of the backpack visible throughout.

Timing: 0.0–0.5 seconds, hold START completely steady. From 0.5–4.5 seconds, apply one continuous, very gentle eased image-plane push-in from scale 1.00 to 1.02 about the exact frame center. From 4.5–5.0 seconds, settle into END and hold. Use a coherent single shot, not a crossfade or dissolve between stills. Maintain a fixed front-facing long-lens product perspective with no orbit, angle change, parallax, focal-length change, tilt or reveal of hidden sides or interior. If a faithful push cannot preserve fine product detail, use a restrained rigid scene transform rather than inventing new geometry.

The backpack, handle, flap, latch, zippers and straps remain physically still and closed. The neutral white background and contact shadow are anchored to the same scene; no new object or horizon appears. Keep the soft upper-left neutral light fixed. Lock exposure, white balance, focus, depth of field, shadow direction and matte fabric appearance for all five seconds. Keep the left desktop region x=5–28%, y=20–75% quiet and empty for optional live HTML copy; generate no lettering or graphics.

Prevent morphing, fabric crawling, seam drift, invented stitching, changing logos or hardware, disappearing straps, duplicated objects, silhouette inflation, geometry drift, flicker, unstable texture, focus pulsing, exposure pumping, moving highlights and gratuitous background motion. No person, prop, product opening, feature demonstration, soundtrack, sound effect, cuts, dissolve, added text, badge, price or watermark. Deliver source footage for a single once-played embedded shot. Do not create a loop or claim the distinct START and END form a seamless loop.
```

## Kullanım ayarları ve durum

- **Yerleşim:** galeri ile özellik anlatımı arasında, gerçek satın alma/bildirim alanını kapatmadan. Öneri; sitenin mevcut kodu değiştirilmedi.
- **Master:** istenen 16:9, tercihen 1920×1080, 5 saniye, 24–30 fps. Gerçek çıktı boyutu ve kare hızı yok; bunlar üretim önerisi.
- **Mobil:** tam yükseklik 9:16 kırpma, 16:9 kaynağın ortadaki yaklaşık %31,6 genişliğini korur. Hedef ürün genişliği iki karede de bunun içinde, fakat gerçek çıktı ölçülmeden güvenli kabul edilmemeli. Sap/kayış kenarı kaybolursa mobilde 16:9 medyayı `contain` ile gösterin veya kaynak fotoğrafı sabit kullanın; görseli esnetmeyin.
- **Metin:** masaüstünde önerilen boş alan x=%5–28, y=%20–75; bu sol alan portre kırpmada korunmaz. Mobil metni medyanın üstüne veya altına canlı HTML olarak koyun. Nihai sayfadaki kontrast ayrıca ölçülmeli.
- **Oynatma:** sessiz ve `playsinline`; varsayılan bir kez oynatma, döngü yok. Üretim sonrası uygun WebM/MP4 sıkıştırması ve küçük poster kullanın. Poster, doğrulandıktan sonra START'tan alınabilir.
- **Erişilebilirlik:** `prefers-reduced-motion` ve veri tasarrufunda sabit poster. Gerçek mobil oynatma veya performans testi yapılmadı.
- **Varlık durumu:** tam iki uç görsel promptu ve bir video promptu hazırlandı. START/END görselleri, video, site entegrasyonu ve uç kare eşleşmesi üretilmedi veya test edilmedi. Kaydedilen JPG'ler yalnız incelenen resmi kaynak fotoğraflarıdır.

## Rubriğe göre öz değerlendirme

| Kontrol | Sonuç | Dayanak / açık sınır |
|---|---|---|
| Kullanıcının mod seçimi | PASS | “Yalnızca promptları hazırla, görsel üretme” korundu; medya üretim çağrısı yok. |
| Kaynak temeli | PASS | Ürün ve marka sayfaları okundu; iki gerçek ürün fotoğrafı görsel incelendi. Stok/CTA bölgesel erişim anına bağlı olarak açıklandı. |
| Siteye uygun kullanım | PASS — tasarım kararı | Ürün değerlendirmesini destekleyen galeri sonrası insert seçildi; fiyat, teslimat, performans iddiası eklenmedi. Sayfada uygulanmış uyum UNVERIFIED. |
| Tam iki uç / süreklilik | PASS — prompt kapsamı | Aynı ürün ve tek %2 hareket tanımlı. Gerçek görsellerin sürekliliği UNVERIFIED. |
| START kalite kapısı | UNVERIFIED | Görsel üretilmedi; sonraki kullanım için kaynakla karşılaştırma talimatı var. Gerçek START kabulü veya END referans bağlama yapılmadı. |
| Fiziksel olarak mümkün hareket | PASS — tasarım | Yalnız görüntü düzleminde küçücük büyüme; yeni yüzey, açılma veya orbit yok. Oluşabilecek ara video kareleri UNVERIFIED. |
| Yerleşim / kırpma | PASS — plan | Orta ürün hedefi, ayrı mobil HTML metni ve contain/still alternatifi var. Gerçek kenarlar ve kontrast UNVERIFIED. |
| Yetenek dürüstlüğü | PASS | Üretim/test iddiası yok; sağlayıcı bayrağı, uç kare garantisi veya döngü vaadi yok. |
| Prompt taşınabilirliği | PASS | Üç blok İngilizce ve sahne/hareket/sabitleri içeriyor. END açıkça gerçek START ekini istiyor; video çift-girdi yeteneği doğrulanmasına bağlı. |
| Erişim ve güven sınırı | PASS | Gerçek URL'ler kullanıldı; giriş, satın alma, yayın, mesaj, ücretli servis veya siteden kod çalıştırma yok. Tam sayfa görsel incelemesinin sınırı belirtildi. |
