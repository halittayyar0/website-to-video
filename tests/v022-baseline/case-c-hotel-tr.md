# Case C — gerçek prompt-only yanıtı

Yalnız promptlar. **Kurgu test fixture'ı:** Gerçek bir otel veya oda temsil edilmiyor; kaynak görsel ve URL yok. Nötr döşenmiş tek oda dışındaki ayrıntılar aşağıdaki sahnenin tasarım tercihleridir. Farklı açılardaki START ve END doğrudan kusursuz döngü kurmaz. Aşağıdaki çekim, aynı sabit gün batımı ışığında küçük bir yatay pan yapar; baştan beri odada bulunan kahvaltı masası ortada daha çok görünür. Sonsuz oynatma için bitmiş videoyu ileri–geri oynatmak gerekir; dönüş noktalarının gerçekten kesintisiz olduğu render ve oynatma testinden sonra söylenebilir.

## START

```text
Create a 16:9 START still for a fictional hotel-room website film. This is a clearly fictional neutral furnished-room fixture, not a representation of an existing hotel, room type, amenity or real property. There is no source property photograph. Use one modest rectangular room with off-white walls, one low double bed with plain beige linen against the back wall, one small wooden bedside table, and one small round wooden breakfast table near the right edge. The breakfast table and a simple breakfast setting already exist in this room; show only its left portion at the right edge in this initial composition. Keep these furnishings fixed throughout the planned shot. Add no other room or exterior amenity.

A single window on the left wall supplies soft warm sunset illumination. The time of day, sunset color, shadows, brightness, exposure and white balance remain fixed, without a changing sky or moving sun. Use a natural 40 mm full-frame camera look at standing height, with level horizon and straight architectural lines. Face the bed from a slightly leftward initial viewing angle; frame for a very small rightward pan later, not a room change. The visible room geometry must be physically coherent. No people, branding, readable text, price, star rating, food-service claim, artificial sunset flare or promotional decorations. This is a still candidate; no factual room fidelity is claimed.
```

## END

```text
Use the generated START image as the primary image reference. Attach the accepted START and create the 16:9 END of the same fictional neutral furnished hotel-room fixture. This is not an existing property or amenity claim. Preserve the same off-white rectangular room, one low double bed with plain beige linen against the back wall, one small wooden bedside table, and the same small round wooden breakfast table with its unchanged simple breakfast setting near the right side. The table was already present in START; do not create, dissolve in, teleport or replace any object.

The only change is a level three-degree rightward pan from the exact same camera position, using the same natural 40 mm full-frame lens and height. This is a slightly different viewing angle in one shot, not a second room or a cut. Reframe enough to make more of the existing breakfast table visible while retaining the bed and room anchors. No dolly, orbit, zoom, geometry deformation or independent furniture movement. Keep left-window sunset illumination, shadow direction and softness, exposure, white balance, surfaces, linens and breakfast setting identical. Do not change time of day or light as a cinematic effect. No people, generated text, logo or new amenity. This END differs from START and is not itself a seamless-loop reset frame.
```

## VIDEO PROMPT

```text
When the chosen video tool supports two endpoint inputs, use the supplied START and END images as first and last frames for a silent five-second 16:9 fictional room film. This is a neutral furnished-room fixture for concept testing, not footage of a real hotel. If two-endpoint input is unsupported, do not execute this two-input prompt as written.

Remain inside one rectangular off-white room for the entire single shot. Keep one low double bed with plain beige linen against the back wall, one small wooden bedside table and one small round wooden breakfast table with its simple breakfast setting at the right side. The breakfast table already exists in START and is partially clipped at the right edge; it becomes more visible around the middle as the framing pans. Nothing appears by materialization, morphing, fade or cut.

Hold the initial slightly leftward angle during 0–0.5 seconds. Pan the fixed-position level camera smoothly three degrees right during 0.5–4.5 seconds, with zero angular velocity at both ends. Hold the final different angle during 4.5–5 seconds. Use a fixed natural 40 mm full-frame lens, unchanged height, focus and exposure. Keep bed and room anchors visible, straight lines stable, and furniture, food, textiles and room geometry fixed. Warm sunset light always enters from the same left-side window with unchanged shadows, white balance and brightness; no day-to-night transition, moving sun, wind or lighting flicker. No zoom, dolly, orbit, new room, disappearing objects, added amenities, people, audio, text or logo.

Render this as one finite forward shot. START and END show different angles, so do not claim the source clip loops seamlessly or force a direct END-to-START reset, dissolve or hidden cut. Intended infinite playback is a later forward-then-reverse presentation of this same finished shot, with the stationary endpoint holds supporting the direction changes. Validate both reversal joins and all intermediate frames before calling the resulting playback seamless.
```

Kullanım: 16:9, beş saniye; gerçek ölçü ve kırpma doğrulanmadı. Mobilde aynı geniş kadrajı oranı korunarak gösterin; kontrolsüz portre kırpımı oda/masayı kesebilir. Metin canlı HTML'de üstte; sessiz satır içi oynatma, START poster ve hareketi azalt/veri tasarrufu için sabit görsel. Araç uç kare desteği bilinmiyor; video üretilmedi, sonsuz döngü ve ara kare sürekliliği test edilmedi.
