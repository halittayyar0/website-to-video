# v0.2.3 bounded forward validation — actual responses

This is a simulated production-response test against the current local skill, not live site research. No browser, image/video generator, paid service, publishing or application mutation was used. Inputs called fixtures below are test premises, not facts verified from the named websites. The separate local-image review used `view_image` on the requested real files.

## 1 — New Codex job, `$website-to-video kutarel.com`, no output choice

Normalized address: `https://kutarel.com`.

Exact next answer:

> Görselleri burada üreteyim mi, yoksa yalnızca kopyalayabileceğiniz görsel ve video promptlarını mı hazırlayayım?
>
> - Görselleri üret
> - Yalnızca promptlar

Next action: wait for an actual mode choice; no media call. Read-only research of that normalized address is permitted while waiting. Status: mode selection pending. The address alone does not authorize generation. No site/brand facts have been verified by this bounded test.

## 2 — Existing prompts-only job, front coat fixture only

Input: `example.com:8443/products/coat?color=black#details`.

Normalized address: `https://example.com:8443/products/coat?color=black#details`.

Exact response:

Yalnızca promptlar hazırlıyorum. Bu testteki tek görsel kaynak, montun önden görüntüsünü gösteren fixture; siteyi canlı incelemedim. `color=black` adres parametresi tek başına ürün renginin doğrulandığı anlamına gelmiyor: görünümde fixture esas alınacak. Önerim, bu ürünün sayfasındaki görsel alanında tam ön görünümden mevcut ön yüz detayına geçen beş saniyelik sessiz bir çekim. Marka, hedef kitle ve CTA henüz doğrulanmadığı için bunlara ilişkin iddia eklemiyorum.

Kaynak kaydı: Kullanıcı/test tarafından sağlanan tek ön mont görseli — ürün kimliği referansı; kaynak dosya adı ve canlı görsel URL'si verilmedi. Yukarıdaki adres bu testte açılmadı. Ön yüz dışındaki arka, iç, yan yapı ve donanım doğrulanmadı. Beyazımsı sade fon, yerleşim ve yaklaşma hareketi tasarım tercihleridir.

Plan: START, montun tüm ön görünümünü merkezde ve kenar paylarıyla gösterir. END, yalnızca başlangıçta görünür olan üst ön yüzü daha yakından gösterir. Arada nesne dönmez; tekdüze görüntü düzlemi ölçeklemesi ve kaydırma ile aynı ön görüntüden detay kadrajına geçilir. Küçük bir global yakınlaşma yerine belirgin tam ürün → detay değişimi amaçlanır; üretilmiş sonuç olmadığı için bu bir tasarım hedefidir.

START prompt:

```text
Create a 16:9 still for the image area of the supplied coat product-detail page. Attach the supplied front-view coat fixture as the source-identity reference. Show exactly one coat in its exact observed front-facing pose, with the entire visible garment centered, including all edges already present in the source, and generous margins. Use a quiet off-white background as an editorial presentation choice; do not add a room, mannequin, person, hanger, accessories, pedestal or scenery. Preserve the source coat's exact observed colors, silhouette, proportions, sleeve shape, front construction, fastening, seams, surface texture and any existing marks. Do not infer black from the URL or add details that the reference does not resolve. Keep any lower-resolution source texture at its supported level of detail rather than inventing weave, stitching or hardware. Use soft diffuse fixed illumination that preserves the reference's readable material appearance, a straight-on camera and no perspective orbit. Keep the garment's upper front as the center of interest; this image will be the start of a continuous crop toward that already visible region. Leave a quiet margin around the object; do not bake any text, slogans, new logos or interface into the image. This is a faithful front-view presentation, not evidence of the coat's unseen back, sides or interior.
```

END prompt:

```text
Use the generated START image as the primary image reference. Attach the accepted START image as the edit target and primary continuity reference; also attach the supplied front-view coat fixture as the source-identity reference. Create a 16:9 ending still for the same coat product-detail insert. Show exactly the same single front-facing coat on the same off-white background with the same fixed soft diffuse illumination and straight-on perspective. Change only the framing through one uniform image-plane scale and translation: enlarge the entire accepted START scene about 1.65 times and place the already visible upper-front region at the center, producing a clearly closer collar/upper-front detail rather than a second full-product view. Choose the crop within source-visible content; do not expose any back, side, interior or concealed fastening. All garment proportions, seam spacing, marks and relative positions scale together; do not keep mark pixel size fixed while enlarging the garment. Preserve the exact accepted START silhouette, construction, observed colors and texture without redrawing or inventing finer weave, stitching or hardware. Do not rotate, change focal perspective, restage, relight, add objects or change the source coat's construction. Include no new text, slogans, logos or interface. The transition must remain attainable by a continuous front-view crop of the same image, with no morphing or dissolve.
```

Video prompt — a target must first be verified to support START and END image inputs:

```text
Create a silent five-second product-detail film using the supplied START still as the first-frame input and the supplied END still as the last-frame input. The scene contains exactly one front-facing coat from the attached source fixture, on a quiet off-white background under fixed soft diffuse illumination. START shows the whole visible garment with generous margins; END shows the already visible collar and upper-front region in a clearly closer crop. Hold START from 0.0 to 0.4 seconds, ease one uniform image-plane scale and translation from 0.4 to 4.6 seconds until the scene is approximately 1.65 times its starting scale and its upper front is centered, then settle into END from 4.6 to 5.0 seconds. This is one planar crop progression with a fixed frontal perspective, not an orbit or a reveal of hidden surfaces. All apparent image-space sizes and spacings, including marks, seams and garment edges, must scale together without independent deformation. Preserve the exact coat count, identity, observed color, front construction, silhouette, fastening, source-supported material detail, background and fixed exposure. Do not invent back, side, interior, microscopic textile or hardware details. No cuts, dissolve, breathing fabric, added object, object rotation, relighting, morphing, disappearing seams, flicker, sound, captions or new logos. End in the supplied END composition without implying a seamless loop.
```

Kullanım: 16:9 master, beş saniye, öneri olarak 24–30 fps; bir kez oynatma veya ayrıca test edilecek ileri/geri scroll eşlemesi. Metni medya dışında canlı HTML olarak yerleştirin. Dikey mobil kullanımda tam montu koruyan ayrı bir kadraj veya START sabit görseli kullanın; 16:9 görüntünün orta 9:16 kırpımının tüm montu koruduğu doğrulanmadı. Poster, sessiz inline gösterim ve reduced-motion/save-data için sabit görsel önerilir. Gerçek görsel boyutları, süreklilik ve video hareketi doğrulanmadı; hiçbir görsel veya video üretilmedi. Hedef yalnızca START kabul ediyorsa, bu iki-girdi promptunu çalıştırmadan önce START-only uyarlaması gerekir; belirli sağlayıcı parametresi varsayılmadı.

Assessment: mode persisted; port/query/fragment preserved; no invented rear view; exactly two complete English image prompts plus a complete conditional dual-endpoint video prompt; no fixture mislabeled as live site evidence.

## 3 — Explicit HTTP, prompts-only, almost still cloth

Input: `http://example.com/quiet?x=1 ; prompts only, 5-second almost still ambient cloth shot, no big zoom`.

Normalized address: `http://example.com/quiet?x=1` (the semicolon and following text are brief instructions, not URL content).

Exact next answer:

> Yalnızca promptlar hazırlayacağım. Beş saniyelik, neredeyse sabit kumaş sahnesini ve büyük yakınlaşma istemediğinizi koruyorum. Önce verdiğiniz HTTP adresindeki sayfayı ve görünür kumaş referansını inceleyeceğim; görüntü kaynağı doğrulandıktan sonra iki görsel promptunu ve video promptunu tamamlayacağım.

Exact next action in an unrestricted production run: read-only inspect `http://example.com/quiet?x=1`, then the homepage for brand context and an actually discovered relevant page/asset as needed. Do not upgrade HTTP, drop `x=1`, ask the mode again, or generate images. In this bounded test no browsing was allowed and no cloth fixture was supplied, so source grounding and completed scene prompts remain pending. Do not invent cloth color, weave, product claims or CTA. When grounded, START/END may intentionally have nearly identical poses; plan only source-supported low-amplitude cloth motion, locked camera and exposure, with no large zoom. Similar endpoints would be consistent with this explicit ambient brief, but would not prove rendered motion.

Assessment: exact explicit brief survives; default perceptible progression does not override it. This is a next-action pass, not a claim of completed website analysis or prompt delivery.

## 4 — Exact 360 degrees back to front, all-sides fixture available

Input: `https://example.com ; prompts only, 5 seconds, front-facing object rotates exactly 360 degrees back to front`.

Normalized address: `https://example.com`.

Exact response:

Yalnızca promptlar. Başlangıçta öne bakan nesne beş saniyede tam 360° döndüğünde yeniden öne bakar; bu istekte çelişki yok. Tüm yanlar fixture ile doğrulanmış kabul ediliyor; bu, canlı site incelemesi yaptığım anlamına gelmiyor. Kamera sabit kalacak, nesne dikey ekseninde saniyede 72° dönecek. START ve END aynı ön pozda olacak; bu bilinçli döngü planı, tamamlanmış videonun kusursuz döngü olduğuna kanıt değil.

Kaynak kaydı: Test tarafından sağlanan ve bütün dönüş yüzlerini doğruladığı belirtilen çok açılı nesne fixture seti — kimlik ve her açı için referans. Canlı sayfa, nesne türü/malzeme adı, satış iddiası ve CTA bu testte doğrulanmadı; promptlar bunları uydurmaz. Yerleşim önerisi, nesnenin ilgili detay sayfasında metinden ayrı bir ürün/nesne alanıdır.

START prompt:

```text
Create a 16:9 starting still for an object-detail website insert. Attach the complete verified all-sides fixture set as source-identity references, with its front view explicitly labeled FRONT. Show exactly one instance of that exact referenced object facing FRONT, centered around its vertical yaw axis, with its whole visible silhouette and enough margins for the widest verified angle of a full rotation. Preserve every source-supported dimension, contour, color, material, seam, mark, fastener and surface feature; invent no details or product capability. Use a quiet neutral background and a fixed soft diffuse studio light setup as presentation choices, with a level, locked straight-on camera and no visible rotating platform or added support hardware. Do not reveal the underside or unseen interior. Set a fixed exposure and keep the object at one constant image scale. This is time 0 of one five-second 360-degree yaw cycle; the initial front pose will be revisited after exactly one full turn. No text, new logo, scenery, person, UI or caption. Use no promotional claims.
```

END prompt:

```text
Use the generated START image as the primary image reference. Attach that exact accepted START image as the edit target and primary continuity reference, and attach the complete verified all-sides fixture set as source-identity references. Produce a 16:9 ending still for the same single object-detail website insert. The object has completed exactly one 360-degree yaw rotation around its fixed vertical center axis in five seconds and now faces the identical FRONT orientation again, not the rear or a three-quarter pose. Return to the same front silhouette, position, image scale, camera, neutral background, fixed light arrangement and exposure as accepted START. Preserve the exact source object geometry, observed material, colors, seams, marks, fasteners and construction. Keep margins that accommodate every verified rotation angle. The repeated pose is intentional for a complete-cycle plan; do not create an unrelated visual difference, extra object, large zoom, camera orbit, relighting or additional text. Do not invent hidden interior or underside geometry. This endpoint records the front pose after the cycle; it does not by itself establish intermediate rotation or a seamless rendered join.
```

Video prompt — use only after verifying that the target supports both image inputs:

```text
Create a silent five-second continuous 360-degree object rotation using the supplied START still as the first-frame input and the supplied END still as the last-frame input. Also use the complete labeled all-sides source fixture set to preserve the object's identity throughout every intermediate angle. Show exactly one referenced object centered on its fixed vertical yaw axis against the same quiet neutral background, with a level locked straight-on camera, constant image scale and fixed soft diffuse studio illumination and exposure. At 0.0 seconds the object faces FRONT. Rotate it at a constant positive yaw speed of exactly 72 degrees per second: 90 degrees at 1.25 seconds, the verified rear at 2.50 seconds, 270 degrees at 3.75 seconds, and exactly 360 degrees with the original FRONT pose at 5.00 seconds. Do not stop at the rear, add a return leg, reverse direction, hold, ease down or accelerate near the join. START and END deliberately show the same front pose after one full cycle; intermediate geometry must follow the verified side and rear references instead of morphing between two matching front photographs. Keep the rotation center, silhouette dimensions, surface markings, seams, hardware and object construction physically consistent. Surface shading may change naturally as the object turns under the spatially fixed lights; do not animate the lights, exposure or background. Do not reveal underside or interior, invent details, create extra objects, wobble, tilt, orbit the camera, zoom, dissolve, cut, flicker, add text or play sound. This is a planned full-cycle source shot. Preserve position, angle, exposure and angular velocity across the eventual loop join; render and inspect all intermediate frames and the join before claiming a seamless loop.
```

Kullanım: Beş saniye ve 16:9 master; döngü için dönüş açısı ve hızını gerçek karelerden kontrol edin. Her açıdaki en geniş siluetin kadraja sığması gerekiyor. Dar mobil kırpım yalnızca gerçek uçlar ve ara açılar incelendikten sonra onaylanabilir; gerekirse ayrı portre kadrajı veya START sabit görseli kullanın. Canlı HTML metnini medya dışında tutun; poster ve hareket azaltma/veri tasarrufu için sabit görsel ekleyin. Gerçek boyutlar, ara açılar, döngü birleşimi ve oynatma doğrulanmadı. Görsel veya video üretilmedi. İki görüntü desteği ve çok açılı kimlik referansları hedef araçta doğrulanmadı; parametre/özellik desteği varsayılmadı.

Assessment: full turn preserved; net end angle is front; no unnecessary rear-end clarification; no tiny push substituted. The all-sides availability is explicitly a fixture premise, not independently checked media in this test.

## 5 — `kutaler.shop` fails DNS and no usable source

Normalized address: `https://kutaler.shop`.

Exact answer after the stated source failure:

> `https://kutaler.shop` adresi DNS nedeniyle açılamadığı ve kullanılabilir başka kaynak bulunmadığı için siteyi analiz edemiyorum. Açılabilir bir URL veya herkese açık sayfa içeriği ve görselini paylaşın. Bu alan adını başka bir marka ya da alan adıyla değiştirmeyeceğim; kaynak olmadan siteye özel görsel/video sonucu hazırlayamıyorum.

Next action: wait for usable public source. No typo correction to `kutarel.com`, no invented brand analysis or completed prompts. If no mode had been chosen before attempted research, that remains an unresolved mode choice too; obtaining an accessible source is the immediate blocker rather than a reason to invent output. DNS failure here is supplied fixture evidence, not a live DNS test performed by this evaluator.

## 6 — `javascript:alert(1)` as website

Normalized address: none; rejected non-web scheme.

Exact answer:

> `javascript:alert(1)` bir HTTP/HTTPS web adresi değil; açmayacağım. Analiz etmem için bir web adresi paylaşın; `kutarel.com` gibi şemasız bir alan adı da olur.

Next action: no navigation and no script execution; wait for an ordinary website address. Do not prepend HTTPS to the entire JavaScript string or treat it as a brand.

## Scope and limitations

The six responses above are produced by this evaluator from the current skill and explicit test premises. They do not count as six independently executed host runs, real website analyses, live DNS verification, successful image generation, successful all-sides rendering, or release-gate completion. Only the separately named local raster files were visually inspected. The supplied coat fixture in case 2 and unspecified all-sides object fixture in case 4 were scenario descriptions, not opened files; the separate crewneck reference was not substituted for either fixture.
