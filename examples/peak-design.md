# E-ticaret — URL-only inceleme ve olumsuz görsel testi

Tek iş girdisi: `https://www.peakdesign.com/products/everyday-backpack`. [Ürün sayfası](https://www.peakdesign.com/products/everyday-backpack) ve [mevcut ürün fotoğrafı](https://cdn.shopify.com/s/files/1/2986/1172/files/everyday-backpack-black-20-1.jpg?crop=center&height=1024&v=1762275581&width=1024) incelendi. Marka günlük kullanım/fotoğraf taşıma çantası sunuyor; ziyaretçi varyantı seçip sepete ekleyebiliyor. Tek yön: ürün ayrıntısının yanında, fotoğraftaki çantayı değiştirmeyen sessiz stüdyo kadrajı. Canlı ürün metni medyanın dışında kalır.

**Görsel araçlı sonuç onaylanmadı.** Bu v0.1.0 geçmiş denemesinde START zaten kaynak fotoğraftaki sade dokuyu değiştirdi; bağımsız inceleme bunu da doğruladı. START yaklaşık %89 yükseklikteydi, istenen %72 değildi. END aynı kusurlu START ile ve iki onarım denemesiyle üretildi; bunlar katalog doğruluğu taşıyor gibi paketlenmedi. v0.2.0'da böyle bir START reddedilir ve END çağrısına geçilmez. Geçmiş çift, yeni START kapısının gerçekten çalıştırıldığına kanıt sayılmaz. Aşağıdaki prompt-only örnek üretim garantisi değildir; gerçek ürüne karşı yeniden kalite kontrol gerekir. Claude uygulaması testi değildir. Codex'te yeni bir URL-only iş bu çıktıdan önce mod seçimi sorusunu alır; mevcut açık prompt-only seçimi varsa tekrar sorulmaz.

İncelenen reddedilmiş START ve END dosyalarının gerçek boyutları 1672×941'dir, tam 16:9 değildir. Bu boyut ölçümü ürün doğruluğu veya yeni kalite kapısının çalışması anlamına gelmez.

## START prompt

```text
Create one START still for a silent embedded product-detail film on the Peak Design Everyday Backpack page. Attach and inspect the official frontal black Everyday Backpack reference from https://cdn.shopify.com/s/files/1/2986/1172/files/everyday-backpack-black-20-1.jpg?crop=center&height=1024&v=1762275581&width=1024 . Preserve the exact existing product silhouette, plain fine woven charcoal-black textile, folded flap, central clasp, seams, zippers, loops, handle and original markings. Do not invent a compartment, change hardware, restyle the fabric or add accessories. Keep its upright frontal orientation on a neutral white studio background with a soft grounded shadow and fixed neutral upper-left illumination. Compose a 16:9 product-page insert with the whole bag and handle within the image and ample margins, no raster type or CTA. The product copy and add-to-cart stay outside the image; on mobile use contain. Aim for about 72 percent bag height, but inspect the actual result rather than assuming the generator obeyed. No people, new logos, props, glow or visible decorative patterns. Return a single START image.
```

## END prompt

```text
Use the generated START image as the primary image reference; attach the actual image. Create the END still for the same five-second silent product-detail insert on the Peak Design Everyday Backpack page. Lock the backpack itself completely: same silhouette, fine plain charcoal-black textile grain, folded flap, central clasp, seams, zippers, loops, handle, markings, position and size. Keep the same 16:9 framing, static camera, neutral upper-left product light and grounded shadow. Change only the empty far-right background with a very faint warm-neutral studio backdrop gradient that fades to original white before reaching the product. This is a separately lit backdrop, not product relighting. No swirls, paisley, decorative weave, added pockets, hardware changes, new words, moving parts, camera movement or crop. Return one END image. Inspect product identity against START and the official photograph; if fabric or hardware changes, reject the pair rather than delivering it as an accurate product view.
```

## Video prompt

```text
Produce one five-second silent embedded product-detail film from the supplied START and END frames. One exact frontal charcoal-black Peak Design Everyday Backpack stands upright on a white seamless studio background with a soft grounded shadow. Preserve the existing product and every visible detail: fine plain woven textile, flap, handle, clasp, seams, zippers, loops and original markings. Lock camera position, perspective, focus, crop, product exposure and its shadow. From 0–0.5 seconds hold START. From 0.5–4.5 seconds bring a very faint warm-neutral illumination into only the far-right empty studio backdrop, matching END; this separate backdrop light must not alter the product. Settle from 4.5–5 seconds. No bag motion, opening, zoom, orbit, shape or fabric morphing, extra accessories, disappearing parts, lettering changes, flicker, cuts, sound or cross-dissolve between reimagined bags. The page retains live HTML product copy and controls outside the image. Recommend 16:9 with mobile contain. Reject the render if product details change. Play once or map to scroll; do not promise a seamless loop for different lighting endpoints.
```

Hedef video aracı belirtilmedi. İki uç kare girişi varsa iki-girdili promptu kullanın. Araç yalnız START kabul ediyorsa aşağıdaki bağımsız promptu kullanın; kesin END eşleşmesi beklemeyin.

### Tek görsel girdisi için video promptu

```text
Use only the attached START image to create one five-second silent embedded product-detail film. One exact frontal charcoal-black Peak Design Everyday Backpack stands upright against the white studio backdrop shown in START. Preserve its fine plain woven fabric, silhouette, flap, handle, clasp, seams, zippers, loops and markings. Keep the camera, framing, product position, product illumination and grounded shadow locked. Hold from0–0.5s. From0.5–4.5s gradually introduce a barely visible warm-neutral backdrop light in the empty far-right margin only, fading to unchanged white before reaching the backpack. From4.5–5s settle at that described lighting state. No other input image is supplied or required. The described last state is guidance, not an enforced frame. Do not repaint fabric, open or move the bag, alter hardware, add objects, change typography, morph geometry, flicker, cut, zoom or orbit. No audio. Recommend16:9 with mobile contain and live product copy outside the media. Reject material or identity drift. Play once or map reversibly to scroll; do not force a loop.
```

Öneri: 5 sn, 24–30 fps kaynak, sessiz, poster ve azaltılmış hareket için resmî ürün fotoğrafı. Video üretilmedi. Başarısız ürün çiftini gizlemek amacıyla başarılı görsel üretim iddiası yapılmadı.
