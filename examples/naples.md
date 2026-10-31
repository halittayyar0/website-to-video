# Gayrimenkul / tatil kiralama — URL-only prompt yolu

Tek iş girdisi: `https://naplesfloridarentals.com/`. Bu denemede prompt-only dalı elle seçildi; gerçek Claude oturumunda çalıştırma yapılmadı. Görsel üretilmedi.

Site, Naples'ta ev kiralamak isteyen ziyaretçiyi evleri incelemeye ve doğrudan rezervasyon akışına götürüyor. Tek yön: koleksiyon girişinde mevcut havuz/avlu fotoğrafından sakin, sessiz bir beş saniyelik film. Bu bir belirli ilan tanıtımı değildir: ana sayfa fotoğrafının hangi ilana ait olduğu doğrulanmadı. Siteye yeni mimari veya tesis eklenmiyor. Üstteki gökyüzü desktop HTML başlığı için düşünülebilir; mobilde metin medyanın dışında ve görüntü contain olmalı.

Kaynaklar: [ana sayfa](https://naplesfloridarentals.com/), [incelenen ilgili ev sayfası](https://naplesfloridarentals.com/naples-4br-kayak-access-heated-waterfall-pool-bbq-huge-yard-orp5b7639bx), [görsel olarak incelenen ana sayfa fotoğrafı](https://uc.orez.io/f/fcbe0311da214edd9cc267479d55d1b4). İlgili ev sayfasının özellikleri bu fotoğrafa aktarılmadı.

## START prompt

```text
Create the START still for a five-second silent collection-introduction film embedded on the Naples Florida Rentals website. Use the existing homepage pool/courtyard photo at https://uc.orez.io/f/fcbe0311da214edd9cc267479d55d1b4 as the attached primary property reference; retrieve and inspect it before generation. Preserve its exact pool outline, pale deck, white fence, planted palms, visible white loungers and blue towels, left-hand covered deck and tiki-bar structure. Do not add rooms, buildings, amenities, beach views or furniture. Retain the source's clear blue sky, soft turquoise water and existing daylight direction. Widescreen 16:9, using a conservative crop of the reference that retains the pool and buildings without inventing unseen edges. Camera fixed at the reference viewpoint. Water begins calm with small natural ripples; existing floats remain in their original locations. No people, raster text, logos or promotional graphics. Reserve the existing quiet upper-sky region for optional live HTML copy on desktop; mobile will use contain and separate copy rather than a destructive portrait crop. This is collection imagery, not evidence that this photo belongs to a particular named listing. Return one single START image.
```

## END prompt

```text
Use the generated START image as the primary image reference and attach it to this request. Create the END still of the same five-second silent Naples Florida Rentals pool/courtyard film. Preserve exactly the same pool outline, pale deck, fence segments, palms, lounger and towel counts, left covered deck, tiki-bar structure, skyline, perspective, 16:9 crop and daylight. Camera is locked. The only permitted change is a slight physically plausible shift of the existing small surface ripples in the turquoise water; existing floats may bob minimally in place but must not travel across the pool. Do not alter architecture, materials, furniture, light direction or shadows. No additions, disappearance, text, people or new amenities. Keep the same quiet sky and image boundaries. Return one END frame, not a montage. If the tool cannot accept START as a reference, do not generate an independent substitute.
```

## Video prompt

```text
Create one five-second silent embedded website film using the supplied START image as the first-frame reference and the supplied END image as the final-frame reference. The scene is the exact photographed Naples Florida Rentals pool courtyard: turquoise pool, pale deck, white boundary fence, palms, white loungers with blue towels, left covered deck and existing tiki-bar structure in fixed daylight. It introduces the rental collection; it must not imply an unverified named property's features. Hold the opening composition for 0–0.5 seconds. From 0.5–4.5 seconds animate only gentle surface ripples toward the END pattern, with any existing floats bobbing minimally in place. Settle gently from 4.5–5 seconds. Lock the camera, lens, exposure, horizon, architecture, furniture, counts, textures and shadow direction. No pan, orbit, zoom, time-of-day change, cuts, photograph dissolve, morphing, vanishing objects, geometry drift, flicker, added rooms or invented amenities. No soundtrack or generated typography. End at the supplied END composition. This is a once-through or scroll-controlled shot; distinct ripple endpoints are not a promised seamless loop. Aspect recommendation is 16:9, with mobile contain and live HTML copy outside the image.
```

İki kare kabul etmeyen bir araçta START'ı tek görsel girdisi yapın; yukarıdaki hareket tarifini kullanın. END yalnız kılavuz olur, zorunlu bitiş eşleşmesi garanti edilmez. Araç belirtilmediği için sağlayıcı parametresi uydurulmadı. Öneri: 5 sn, sessiz, 24–30 fps kaynak, hafif poster; kaydırma için ileri/geri gerçek görüntü testi, azaltılmış harekette sabit fotoğraf. Video üretilmedi veya test edilmedi.
