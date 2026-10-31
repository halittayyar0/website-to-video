# Linear — promptlar, tek başlangıç görseliyle video

Mod: **Yalnız promptlar.** Görsel/video üretilmedi. Araştırma: 31 Ekim 2026. Aynı gün güncel skill ile yalnız teslim aşaması yeniden yürütüldü; yeni araştırma veya üretim yapılmadı. Kullanacağınız aracın yalnız START kabul ettiği bilgisi esas alındı; bu araç için kullanılacak tam metin aşağıdaki **VIDEO PROMPT — yalnız START girdisi** bloğudur. END, kompozisyon hedefini anlatan ikinci görsel promptudur; video aracına yüklenmeyecek ve son kareyi zorlamayacaktır.

Linear, ürün geliştirme ekipleri için planlama ve iş yürütme sunuyor; ana sayfada “Sign up / Get started” ve satış iletişimi çağrıları var. Planlama sayfası projeleri, dokümanları ve bağımlılıkları bir arada ele alıyor. [Ana sayfa](https://linear.app/), [Planlama](https://linear.app/plan)

Tek yaratıcı yön: ana sayfanın planlama bölümündeki açıklamanın altında, gerçek ürün gösterimini örtmeden kullanılacak beş saniyelik sessiz bir **temsili planlama illüstrasyonu**. Siyah zeminde üç kısa planlama rayı, ortak bir bağlantı omurgası ve üç düğüm; bu şekiller Linear ekranı, gerçek kullanıcı verisi veya bir otomasyonun çalıştığına dair kanıt değildir. Koyu yüzey, ince ayrım çizgileri ve küçük mor vurgu incelenen resmi görselle ilişkili; şekillerin sayısı, konumu ve %2 yakınlaşma tasarım tercihidir. Amaç, ziyaretçinin planlama bölümünü sakin biçimde okumasına yardımcı olmak; kayıt CTA'sı canlı HTML olarak sayfada kalır.

## Kaynak kaydı ve sınırlar

| İncelenen kaynak | Doğrulanan / sınır |
|---|---|
| [linear.app](https://linear.app/) | Ana sayfa metni, ürün alanları ve CTA'lar okundu. Tam tarayıcı render'ı, tipografi ve responsive davranış incelenmedi. |
| [linear.app/plan](https://linear.app/plan) | Ana sayfadaki gerçek bağlantı izlenerek projeler, dokümanlar ve planlama bağlamı okundu. Filmde bunlara yeni bir işlev eklenmiyor. |
| [linear.app/build](https://linear.app/build) | Ana sayfadaki gerçek bağlantıdan ekip/agent iş yürütme bağlamı okundu. Reklam filmi veya özellik animasyonu yapılmıyor. |
| [Resmi ana sayfa dekoratif varlığı 09](https://linear.app/cdn-cgi/imagedelivery/fO02fVwohEs9s9UHFwon6A/6600ca96-e49b-4fd9-c03a-7979faddad00/f=auto,fit=scale-down,metadata=none,width=2560) | Dosya indirilip görsel açıldı. Çok koyu ve kısmen saydam dekoratif şekiller; görüntüleyicinin yeşil görünen saydamlık zemini marka rengi olarak alınmadı. Tek başına bütün hero görünümünü kanıtlamaz. |
| [Resmi ana sayfa dekoratif varlığı 10](https://linear.app/cdn-cgi/imagedelivery/fO02fVwohEs9s9UHFwon6A/c7fa8f5f-d439-4329-6a65-de549b51e300/f=auto,fit=scale-down,metadata=none,width=2560) | Dosya indirilip görsel açıldı. Koyu zemin ve alt orta bölgede beyaz/gri yumuşak ışık alanı görüldü; bütün sayfa kompozisyonu değil. |
| [Resmi Plan/Projects görseli](https://linear.app/cdn-cgi/imagedelivery/fO02fVwohEs9s9UHFwon6A/028734bb-2e5c-463d-c4ef-702eef293500/f=auto,fit=scale-down,metadata=none) | Dosya indirilip görsel açıldı. “UI Refresh” proje örneği, koyu arka plan, açık/gri metin, ince sınırlar ve küçük mor/turuncu vurgular görüldü. Yalnız yoğunluk/palet referansı; metinler, avatarlar veya ekran yapısı yeni görselde kopyalanmayacak. |

Not: Web aracının döndürdüğü yüzde kodlu CDN URL'leri ilk yerel indirme denemesinde “malformed URL” verdi. Aynı bağlantıların eşdeğer, kodu çözülmüş parametre yazımıyla normal indirme başarılı oldu; erişim kontrolü aşılmadı. Kaynak dosyalar üretim çıktısı değildir.

## Süreklilik kilidi

Bir kompakt temsili planlama motifi; tam üç yatay ray, bir dikey bağlantı omurgası, tam üç küçük yuvarlak düğüm. Koyu nötr zemin ve ince gri çizgiler; yalnız orta düğüm soluk mor. Önden sabit ortografik görünüm, üst soldan sabit yumuşak ışık, aynı keskinlik ve pozlama. Kompozisyon hedefi x=%38–62, y=%30–70; üç rayın y merkezleri %35, %50, %65, omurga x=%40. Tek fark, bütün sahnenin merkez etrafında %2 büyümesi; çizgi kalınlıkları, düğüm çapları ve aralıklar dahil görüntüdeki bütün ölçüler aynı 1,02 katsayısıyla büyür. Oranlar ve göreli sahne geometrisi korunur; hiçbir parça bağımsız deforme olmaz. Metin, arayüz, sayı, logo, ekran, imleç, yeni düğüm veya durum değişimi yok.

## START — tam İngilizce görsel promptu

```text
Create the START still for a silent five-second embedded editorial film in the planning section of Linear's homepage, below the planning explanation and separate from the real software demonstration. Output a 16:9 landscape image, preferably 1920 x 1080 if supported. This is a clearly nonliteral illustration of connected product planning, not a screenshot of Linear, not a feature demonstration and not customer data.

Create one compact, precise planning motif on a matte near-black background: exactly three thin horizontal rounded rails, one thin vertical connecting spine and exactly three small circular nodes where the spine meets the rails. The spine sits at x=40% and runs from y=35% to y=65%. The upper rail is centered at y=35% and extends from x=40% to x=60%; the middle rail is centered at y=50% and extends from x=40% to x=62%; the lower rail is centered at y=65% and extends from x=40% to x=58%. Nodes sit at the three intersections. The upper and lower nodes are neutral pale gray, and the middle node is muted violet. Keep the complete motif inside approximately x=38–62%, y=30–70%. This geometry is an editorial design choice and must not resemble an actual application window, dashboard or chart.

Use quiet charcoal surfaces, fine low-contrast gray boundaries and restrained pale gray highlights. Keep each rail slim and the nodes small; no glass, chrome, glossy plastic, neon bloom or dramatic glow. View straight on with a fixed orthographic camera and no perspective convergence or visible horizon. A soft neutral upper-left light gives only subtle relief; all illumination, focus and exposure remain stable. The visual density should be restrained enough to sit beside real product information.

For optional palette and density reference only, attach this official Linear Projects image: https://linear.app/cdn-cgi/imagedelivery/fO02fVwohEs9s9UHFwon6A/028734bb-2e5c-463d-c4ef-702eef293500/f=auto,fit=scale-down,metadata=none . Do not copy its text, people, avatars, icons, UI layout, feature data or project content. This is a style reference, not a product-identity or interface reference. The new image contains no text, glyph, number, logo, watermark, cursor, button, browser chrome, device, person or extra object.

Keep the desktop copy-safe area x=5–28%, y=20–75% empty and near-black. Any explanation or CTA belongs in live HTML outside the generated image. This still is the beginning of one shot; nothing moves or changes state.
```

## END — tam İngilizce görsel promptu

Bu görsel, tek-girdi video aracına eklenmeyecek; hedef kompozisyonu gözle karşılaştırmak için kullanılabilir.

```text
Use the generated START image as the primary image reference. Attach the actual accepted START still as the edit target and continuity anchor. Produce the END still of the same five-second editorial planning film for Linear's homepage. Keep the exact same 16:9 canvas and dimensions as START. This is a nonliteral planning illustration, not actual Linear UI, customer data or a feature demonstration.

The scene contains one compact motif on a matte near-black background: exactly three slim horizontal rounded rails, one thin vertical connecting spine and exactly three small circular nodes at the intersections. Before the planned enlargement, the spine is at x=40% from y=35% to y=65%; the rails are at y=35%, y=50% and y=65%, extending respectively from x=40% to x=60%, x=62% and x=58%. The upper and lower nodes remain pale gray; only the middle node is muted violet. Preserve START's proportions, relative scene geometry, overlaps, matte surfaces, fine gray boundaries and muted highlight colors. Every apparent image-space dimension, including rail thicknesses, corner radii, circle sizes and spacing, must scale uniformly with the complete scene; no part deforms or changes independently. There are no words, numbers, UI controls, labels, logos, avatars or real project content.

Make only one small change: enlarge the entire START scene by 2% about the exact frame center, a uniform image-plane scale from 1.00 to 1.02. At END, every apparent image-space size, line thickness and spacing is exactly 1.02 times its START value, with all relative proportions fixed. Keep the motif centered within the central portion of the frame, fully visible with margins. Do not move a node along a rail, change a status, add connections, redraw the motif, change object count or reveal hidden geometry. The straight-on orthographic view stays fixed: no orbit, tilt, parallax, perspective change or focal-length change.

Keep the same matte near-black background, soft neutral upper-left lighting, shadow or relief direction, exposure, white balance, focus and subtle depth. Maintain the quiet empty desktop copy region x=5–28%, y=20–75%. No new object, screen, cursor, person, text, number, logo, watermark, glow pulse, light sweep or color transition. This is a slightly closer instant in the same shot, not an alternate composition or a crossfade. Use the official Linear Projects image, if needed, only as a secondary palette reference: https://linear.app/cdn-cgi/imagedelivery/fO02fVwohEs9s9UHFwon6A/028734bb-2e5c-463d-c4ef-702eef293500/f=auto,fit=scale-down,metadata=none . Never copy or invent its interface.
```

## VIDEO PROMPT — yalnız START girdisi

Video aracına **yalnız gerçek START görselini ekleyin** ve aşağıdaki bloğu kullanın. END'in tarif edilen görünümü bir rehberdir; araçta END alanı olmadığı için birebir son kare eşleşmesi zorlanamaz.

```text
Use the attached START image as the sole image input. Create a silent five-second 16:9 embedded editorial film for the planning section of Linear's homepage. No second image or last-frame input is supplied or required. The desired end state described below is visual guidance, not an enforced endpoint.

The START scene is one compact nonliteral planning motif on a matte near-black background: exactly three slim horizontal rounded rails, one thin vertical connecting spine and exactly three small circular intersection nodes. The spine is initially around x=40%, y=35–65%; the rail centers are y=35%, y=50% and y=65%, extending from x=40% to x=60%, x=62% and x=58%, respectively. The upper and lower nodes are pale gray, and the middle node is muted violet. Maintain the attached START's exact geometry when its actual pixels differ slightly from these intended coordinates. This is a clearly editorial illustration, not a Linear software interface, customer data, measured chart or demonstration of an automation.

From 0.0–0.5 seconds, hold the supplied START completely steady. From 0.5–4.5 seconds, make one very gentle eased image-plane push-in, enlarging the whole scene from scale 1.00 to approximately 1.02 about the exact frame center. From 4.5–5.0 seconds, settle and hold this slightly closer view. The desired final composition is simply the same unchanged motif, about 2% larger than START, with all rails, the spine and all three nodes still fully visible. Do not create or request another reference image to reach it. Exact final-frame matching is not assumed.

The camera remains straight-on and orthographic with no orbit, tilt, lateral movement, parallax, perspective change or focal-length change. Preserve the count, topology, proportions, overlap relationships and relative scene geometry of every shape. As the complete scene scales from 1.00 to approximately 1.02, every apparent image-space size, spacing, corner radius, line thickness and circle diameter scales by the same factor; none stays separately fixed in pixels or deforms independently. No node travels along a rail, no connection is added, and no shape changes state. Use one coherent uniform scaling transform of the complete scene rather than morphing or a dissolve.

Keep the matte charcoal surfaces, fine low-contrast gray boundaries, pale gray nodes, muted violet middle node and near-black background unchanged. Lock the soft neutral upper-left light, subtle relief, shadow direction, exposure, white balance, focus and depth for the whole shot. Keep the desktop copy region x=5–28%, y=20–75% quiet and empty for live HTML. No text, number, glyph, logo, watermark, browser window, screen, button, cursor, avatar, person, added object or feature claim. Prevent geometry drift, disappearing rails, duplicated nodes, nonuniform thickness changes, texture crawling, flicker, glow pulses, moving highlights, exposure pumping and gratuitous background motion. No cut, crossfade, audio or sound effect. This is a once-played shot with distinct beginning and slightly enlarged ending, not a seamless loop.
```

## Kullanım önerileri ve gerçek durum

- **Master:** istenen 16:9, tercihen 1920×1080; 5 saniye ve 24–30 fps önerilir. Gerçek üretilmiş dosya boyutu, oranı veya kare hızı yok. Bunlar sağlayıcı parametresi değildir.
- **Yerleşim:** ana sayfanın planlama açıklaması altında küçük, metne eşlik eden medya. Ürün ekranı yerine geçmesin; temsili niteliği açıklamada belirtilebilir.
- **Kırpma:** hedef motif x=%38–62. 16:9 kaynaktan 9:16 tam yükseklik kırpma yalnız orta yaklaşık %31,6 genişliği tutar. Hedefin sığması tasarım niyetidir; gerçek START/END kenarları doğrulanana kadar mobilde 16:9 `contain` veya sabit poster kullanın. Sol metin alanı portrede korunmaz; mobil metin medyanın üstünde/altında HTML olsun.
- **Oynatma:** sessiz, `playsinline`, bir kez; döngü yok. Kabul edilmiş START'tan poster, çıktı incelendikten sonra uygun WebM/MP4 sıkıştırma. `prefers-reduced-motion` ve veri tasarrufunda sabit poster. Bu iş scroll uygulaması talep etmiyor.
- **Tek-girdi sınırı:** END promptu ve görseli yalnız hedef/review içindir; gerçek video aracına yüklenmez. Son kompozisyon metinle yönlendirilir, garanti edilmez. Sağlayıcı adı, hayali parametre veya video testi iddiası yok.
- **Durum:** tam iki görsel promptu ve bağımsız tek-girdi video promptu hazır. Görsel/video üretimi, gerçek süreklilik, ara kare, kontrast, mobil oynatma ve entegrasyon testi yapılmadı. İndirilen dosyalar yalnız resmi kaynak incelemesidir.

## Rubrik ve bağımsız kopyalanabilirlik denetimi

| Kontrol | Sonuç | Gerekçe |
|---|---|---|
| Mod seçimi | PASS | Açık prompt-only seçimi korundu; üretim veya ücretli araç çağrısı yok. |
| Kaynak temeli | PASS | Gerçek ana sayfa, iki ilgili sayfa ve üç gerçek kaynak görsel incelendi. |
| Siteye uygunluk | PASS — konsept düzeyi | Planlama bölümüne bağlı; gerçek UI veya kanıtlanmamış özellik gösterimi değil. Nihai sayfa uyumu UNVERIFIED. |
| Tam iki uç | PASS — teslim kapsamı | Yalnız START ve END görsel promptu var; ayrı sahne/üçüncü uç yok. Gerçek görsel sürekliliği UNVERIFIED. |
| START kapısı | UNVERIFIED | Üretilmiş görsel yok; gerçek kabul, ret veya START-reference edit yürütülmedi. |
| Uygulanabilir hareket | PASS — plan | Tek %2 görüntü düzlemi büyümesi; durum değişimi, geometri açığa çıkarma veya orbit yok. Video sonucu UNVERIFIED. |
| Kırpma ve metin | PASS — plan | Merkez hedefi, portre sınırı, HTML metin ve contain/still alternatifi açık. Gerçek piksel/kontrast UNVERIFIED. |
| START bloğu tek başına | PASS | Konum, sahne, palet, ışık, kaynak rolü, sayılar ve yasaklar blok içinde. |
| END bloğu tek başına | PASS | START'ı birincil referans olarak açıkça istiyor; sahne ve sabitler içeride; yalnız bir küçük değişim. |
| Tek-girdi video bloğu tek başına | PASS | Yalnız START eki istiyor; son durumu metinle eksiksiz tarif ediyor; tedarik edilmemiş END'e, başka paragrafa veya ikinci kare alanına ihtiyaç yok. |
| Yetenek dürüstlüğü | PASS | Son durumun zorlanmadığı açık; görüntü/video üretildiği, gerçek süreklilik doğrulandığı veya döngünün kusursuz olduğu söylenmiyor. |
| Erişim/güven sınırı | PASS | Yalnız normal web ve kaynak görsel okuması; CUA/UI, giriş, dış yazma, satın alma, yayın ve site kodunu yerel çalıştırma yok. |
