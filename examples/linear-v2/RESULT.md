# Linear, yeni v0.2.0 görsel araçlı koşu

31 Ekim 2026. Güncel ana sayfa, planlama sayfası ve üç resmî varlık incelendi. Koyu yüzey, yumuşak beyaz ışık ve küçük mor vurgu bu kaynaklara dayanır. Üç grafit ray ve tek mor küre, planlama içeriğine eşlik eden **soyut bir illüstrasyondur**; gerçek Linear ekranı veya özellik kanıtı değildir. Kaynak sayfalar: [ana sayfa](https://linear.app/), [planlama](https://linear.app/plan).

Gerçek dosyalar: [START.png](START.png), [END.png](END.png). İkisi de 1672×941, yaklaşık 16:9. START açılıp kabul edildi; her END çağrısında bu gerçek START referans olarak bağlandı. Bir START, bir END ve iki END onarımı olmak üzere dört çağrı yapıldı. Seçilen END ikinci END denemesidir; üçüncü deneme daha fazla yarar sağlamadı. Ürün kumaşı başarısız Peak denemesinden bu soyut işe geçilmedi: bu, ayrı Linear URL'sinin baştan seçilmiş ayrı konseptidir.

İlk tasarım hedefi %2 büyümeydi. Seçilen END'in eşleşen özelliklerine dayalı yaklaşık ölçek %3,8'dir; bunun tam %2 olduğu söylenmez. Görsel inceleme nesne sayısını, sahne kimliğini, malzemeyi ve ışığı koruduğunu gördü. Aynı sakin yakınlaşma konsepti, gerçek son kadraja göre güncellendi. Sayısal eşleştirme tek başına kalite veya piksel-identik ölçek kanıtı değildir; ara video üretilmedi.

## START üretiminde gerçekten kullanılan İngilizce prompt

```text
Use case: stylized-concept.
Asset type: START still of an abstract editorial illustration for an embedded Linear planning-section film, NOT a product screenshot or feature demonstration.
Input image 1 is an actually inspected official Linear homepage glow asset, a near-black field with a broad soft white elliptical glow near the bottom. Its role is lighting/palette inspiration only, not a subject to copy or factual UI.
Create a restrained 16:9 1792x1008 dark studio image of exactly three short solid extruded graphite rectangular rails lying parallel on a matte near-black horizontal plane. The rails are simple real sculptural bars, NOT UI cards, panels, dashboards, or text rows. Each has the same width, length and shallow height, a satin graphite top, sharply machined edges and a dark sidewall. They run left-to-right with their long axes parallel, seen from a fixed modest overhead three-quarter camera so top planes and front sidewalls are visible. Arrange them as three evenly spaced parallel lanes, a compact group centered around x60%, y60%, occupying x42-78% and y42-77%. Leave x0-32% and the top quarter quiet near-black for possible live HTML copy outside the artwork.
A single small solid pale-violet ceramic sphere rests motionless at the midpoint of the MIDDLE rail only. Exactly one sphere, exactly three rails, no other objects, connectors or markings. One broad soft white area light from upper left and a very faint gray-white elliptical ground glow, inspired by the source, illuminate thin edge highlights without fog or beams. Palette: near-black, graphite, soft silver-white and a restrained pale violet accent. Matte black seamless background; no horizon line, gradients or UI grid beyond physically soft studio falloff.
This illustration is a nonliteral metaphor for coordinated product work and ordered progress. No actual app screens, logos, letters, numbers, charts, data, browser frames, icons, arrows or invented capabilities. No extra shapes, particles, neon, visible text or symbols. First moment of a single locked shot; later END changes only a 2% image-plane push. Preserve crisp countable geometry and quiet exposure.
```

## İlk END isteğinin İngilizce promptu

Bu, gerçek ilk çağrının tekrarlanabilir isteğidir; istenen %2 sonucu garanti etmedi. Onarımların tam metinleri ve referans rolleri [çağrı kaydında](../../tests/linear-generation-v2.json) bulunur.

```text
Use case: precise-object-edit.
Asset type: END still for a five-second abstract editorial illustration within Linear's planning-section content, not a screenshot or feature demonstration.
Use the generated START image as the primary image reference. Attach the actual accepted START.png as the sole primary continuity reference and edit target.
The concrete scene is exactly three equal solid graphite rails lying parallel and evenly spaced on a matte near-black horizontal studio plane, with exactly one small pale-violet ceramic sphere resting at the midpoint of the middle rail. The rails have satin top planes, thin machined edge bevels and dark front sidewalls, viewed by one fixed modest overhead three-quarter camera. Preserve the complete group at right-center, its exact proportions, sphere placement relative to the middle rail, materials, shadows, white upper-left area light, broad soft ground glow, black seamless field, exposure and focus.
Match the actual 1672x941 near-16:9 START canvas. Make only a very subtle approximately 3.8% uniform image-plane scene enlargement about the object-group center to match the reviewed END.png. Keep all proportions and scene-relative geometry fixed while all apparent image-space dimensions, line widths, spacing and existing shadows scale together. No independent deformation or motion, orbit, pan, tilt, newly revealed surfaces, extra bevels, moving sphere, changed materials, relighting or added highlights. No UI, app panels, charts, text, numbers, data, logos, graphics, arrows or additional objects. Retain the complete landscape subject; copy stays as live HTML outside the artwork.
```

## Gerçek son kadraja göre güncellenmiş VIDEO PROMPT

Hedef aracın iki uç görseli kabul ettiği doğrulanırsa kullanılır. Araç yalnız START kabul ederse bu blok doğrudan kopyalanmaz; skill tek-girdi için bağımsız bir video promptu hazırlar.

```text
Create a silent five-second embedded editorial film for Linear's planning-section content, using START.png and END.png as first and final image references only when the chosen video tool has verified support for both endpoint inputs. This scene is an explicitly abstract illustration of coordinated product work, not a representation of actual software UI or measured performance. Both supplied reviewed stills are 1672x941, approximately 16:9. Do not invent provider-specific flags.
The scene contains exactly three short solid extruded graphite rectangular rails lying parallel and evenly spaced on a matte near-black plane. All three have matching proportions, satin graphite top planes, thin machined edge bevels, dark front sidewalls and unchanged end faces. Their long axes run left-to-right, viewed by one fixed modest overhead three-quarter camera. The compact group sits at right-center with a broad quiet black upper region. Exactly one small pale-violet ceramic sphere rests motionless at the midpoint of the middle rail. A broad soft white area light from upper left produces thin edge highlights, stable soft shadows and a gray-white ground glow against a seamless near-black background.
Hold START completely still from 0.0 to 0.5 seconds. From 0.5 to 4.5 seconds make a very slow smoothly eased image-plane push toward the object-group anchor, reaching the supplied END framing at approximately 3.8% larger apparent scene scale. The reviewed END is the framing guide; do not describe this as an exact 2% move. From 4.5 to 5.0 seconds settle and hold END. Rails and sphere remain stationary relative to one another and the plane. Keep proportions, camera axis, lens perspective, object count, relative spacing, sphere contact position, material identity, light direction, exposure, focus and background stable. During the allowed uniform scene transform, all apparent image-space dimensions, line widths, spacing and existing shadows scale together; prevent independent deformation, unintended rotation, orbit, parallax or new visible surfaces.
No app panels, UI elements, charts, measurements, lettering, numbers, logos, arrows, particles, fog or extra shapes. Prevent morphing, disappearing or duplicated objects, changing bevels, texture crawling, flicker, geometry drift, relighting and gratuitous movement. Use one coherent continuous shot without a cut, crossfade or dissolve. No audio and no seamless-loop promise. If the selected tool accepts only START, prepare a complete compatible START-only prompt before rendering, with this end state described in prose; END would then be a guide rather than an enforced endpoint. The reviewed still pair does not prove intermediate-frame fidelity or playback performance.
```

## Kullanım ve kanıt sınırı

Öneri: planlama açıklaması yanında/altında beş saniyelik sessiz medya. Mobilde bütün rayları koruyan landscape `contain` veya sabit START kullanın; portre cover kenarları keser. Başlık/CTA medyanın dışında canlı HTML olsun. Üst bölge karanlık ve sakindir, fakat uygulanmış metin kontrastı test edilmedi. Poster ve reduced-motion/save-data görünümü START olabilir. Bir kez oynatma veya gerçek görsel ileri/geri testinden sonra scroll; döngü garantisi yok.

Bu, üretilmiş ve görsel incelenmiş iki sabit karedir. Video, ara kareler, hedef sağlayıcı girdisi, canlı sayfa yerleşimi ve telefon performansı test edilmedi. Kaynakların tamamı tarayıcıda render edilmedi; gerçek ürün görsel varlıkları ayrı açıldı.
