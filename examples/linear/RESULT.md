# Yazılım ürünü — URL-only görsel araçlı deneme

Tek iş girdisi: `https://linear.app/`. [Ana sayfa](https://linear.app/) ve [planlama sayfası](https://linear.app/plan) incelendi; ana sayfa yerel Chrome'da da görsel olarak açıldı. Linear ekiplerin ürün planlama ve geliştirme işlerini yönetmesine odaklanıyor; belirgin ziyaretçi eylemi kaydolmak. Gerçek sayfa koyu nötr yüzeyler, ince çizgiler, beyaz yazılar ve küçük sarı durum işaretleri kullanıyor.

Seçilen tek yön, planlama açıklamasının yanında yer alabilecek bir **soyut iş akışı illüstrasyonu**: üç sabit kart ve soldan ortaya ilerleyen tek sarı işaret. Bu bir gerçek Linear ekran görüntüsü veya doğrulanmamış özellik iddiası değildir. Mevcut ürün arayüzünün yerini almaz. İki kare gerçekten üretildi; END için START dosyası referans olarak kullanıldı. Görüntülerde üç kart, altı çizgi, bağlayıcı ve tek sarı işaret görüldü; yalnız işaretin yeri değişiyor. Video henüz üretilmedi.

START: [start.png](start.png). END: [end.png](end.png). Gerçek ölçüler 1672×941; yaklaşık 16:9. Bunlar v0.1.0'da üretilmiş ve v0.2.0 incelemesinde yeniden değerlendirilmiş sabit görüntülerdir; yeni sürümde yeniden üretim yapıldı iddiası yoktur. Codex'teki yeni URL-only iş mod sorusunu alır; bu sonuç, üretim seçildikten sonraki çıktı örneğidir.

## START prompt

```text
Create the START still of a five-second silent embedded workflow illustration for Linear's product-development website, placed below the planning explanation beside live HTML copy and sign-up navigation. Use a restrained near-black charcoal background, thin neutral-gray outlines, off-white strokes and one small warm-yellow status accent matching the inspected site's visual language. A flat editorial diagram, not a real UI screenshot or an advertisement. In a 16:9 frame show exactly three identical small rounded rectangular cards in one horizontal row, centered around x=34%,50%,66% and y=53%. Each card contains exactly two short off-white horizontal strokes with no text. A thin gray horizontal connector links the three cards behind them. Exactly one small warm-yellow circular marker sits below the left card, approximately x=34%,y=58.5%. Keep the top40% quiet for optional live HTML copy. No words, logos, buttons, people, numbers, extra cards, extra dots, particles or perspective. All objects except the marker will be invariant in END. Mobile will use contain, not a portrait crop that loses the outside cards. Return one single START image.
```

## END prompt

```text
Use the generated START image as the primary strict reference and attach the actual image. Create the END still for the same silent Linear-inspired abstract workflow illustration, not a fake software screenshot. Make exactly one edit: move the single warm-yellow marker horizontally from below the left card to below the center card at x=50%, retaining its original y coordinate near58.5%, diameter, color and brightness. Remove the previous dot cleanly so exactly one dot remains. Preserve the exact three card outlines, their positions and sizes, all six white strokes, the connector and charcoal background. Locked camera and same16:9 image boundaries. No zoom, orbit, perspective, new cards, labels, glow, extra nodes, morphing or lighting changes. Keep the quiet upper40% available for live HTML copy; mobile uses contain. Return one single END image.
```

## Video prompt

```text
Create one five-second silent embedded web illustration using supplied START as the first frame and supplied END as the last-frame reference. The scene is a flat charcoal diagram with exactly three fixed gray-outlined rounded rectangular cards in a horizontal row around34%,50%,66% of the image width, two short off-white strokes inside each card, one fine gray connecting line, and exactly one small warm-yellow circular status marker. This is an abstract illustration of issue flow for Linear's planning explanation, not actual software UI or a claimed product feature. Lock all cards, six strokes, connector, background, camera, exposure and aspect. Hold START from0–0.5s. From0.5–4.5s translate only the single marker in a straight horizontal path from below the left card to below the center card, preserving its y coordinate near58.5%, size and color; ease gently at both ends. Hold END from4.5–5s. No duplicates, disappearing marker, new objects, card deformation, geometry drift, morphing, camera motion, cuts, flicker, text or sound. Match the supplied END position. Recommend16:9, top40% quiet for optional live HTML copy, and contain on mobile. Play once or map the one shot reversibly to scroll; the different dot endpoints are not a seamless loop.
```

İki kare kabul etmeyen araç için aşağıdaki START-only promptu kullanın. Tarif edilen bitiş yalnız kılavuzdur; zorunlu eşleşme iddiası yoktur.

### Tek görsel girdisi için video promptu

```text
Use only the attached START image to create one five-second silent abstract workflow illustration for the planning explanation on Linear's website. This is not actual software UI. Preserve the exact three fixed gray-outlined rounded cards, six white strokes, horizontal connector and charcoal background. Keep camera, aspect, framing and exposure locked. There is exactly one small warm-yellow circular progress marker, initially below the left card. Hold0–0.5s, then ease only that marker horizontally to a position directly below the center card from0.5–4.5s, preserving its original y coordinate near58.5percent of the image height, diameter and color. Settle4.5–5s. No second image is supplied or required; this end state is a textual target, not an enforced final frame. No duplicate or disappearing marker, changing cards or strokes, extra nodes, new text, morphing, geometry drift, flicker, cuts, audio, zoom or orbit. Recommend16:9 and mobile contain, with live HTML copy in the quiet upper region or outside the image. Play once or map the one shot reversibly to scroll; do not loop different marker endpoints.
```

Sağlayıcıya özel parametre kullanılmadı. Öneri: 5 saniye, sessiz, 24–30 fps kaynak; hafif START posteri, mobil contain, başlık/CTA HTML olarak medyanın dışında veya üstteki sakin alanda. Kaydırmalı uygulama ayrıca gerçek ileri/geri görüntü ve mobil performans testi gerektirir; video dosyası veya scroll motoru bu örnekte üretilmedi.
