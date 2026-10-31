# Production contract

Choose only decisions that support this site's visitor action. A shopping product page may need an accurate product-detail insert with no overlay, rather than a lifestyle hero. A rental listing needs faithful property photography, not an invented villa. A software page may use a verified screen recording; if choosing an abstract workflow, label it as an illustration and do not fabricate actual UI, metrics or features.

## Endpoint continuity

Keep a concise continuity record before calling a generator: source image URL or file, what it actually depicts, START file/asset ID, which details must match, the one allowed change, and the intended display/crop. Use the exact accepted START on END calls. A matching brand palette or similar silhouette is insufficient for a literal product/property. If the homepage image cannot be mapped to a named listing, keep it at collection level or verify the mapping; do not transfer another page's amenities onto it.

List subject count, recognizable anchors, horizon/vanishing points, fixed light and materials. Describe only a small feasible change: a 2–4% slow camera push, a very slight shadow/water movement, or a small controlled subject motion. Do not combine a camera orbit, focal-length change, lighting transition and object action in five seconds. Moving toward a detailed product can reveal unseen geometry; avoid this when the source cannot verify it. Prefer a small image-plane push that does not invent hidden sides.

For an image-plane scale, keep proportions and relative scene geometry fixed while all apparent image-space sizes, line widths and spacing scale together. Do not also demand pixel-identical sizes or forbid the intended uniform size change; prohibit independent deformation instead. Describe this as a uniform scene transform.

Prefer the smallest necessary edit to existing faithful imagery over an expansive restaging that invents surroundings. Label each attached image's role (source identity, edit target, or accepted START), not just its filename. For a repair, say which defect changes and what stays fixed. Do not compensate for a failed literal product rendering by selecting a different abstract concept. If exact identity is important and the available tool keeps redrawing it, report that this output is not suitable for that use rather than promising pixel preservation through prompting.

Compose the key subject inside the central crop shared by the intended desktop and mobile layouts, with reasonable margins. For a full-height 9:16 crop of a 16:9 image, only about the middle 32% of the width remains; do not casually promise that widely spaced objects survive it. Keep text as live HTML, not generated raster lettering. Name the exact copy-safe region and whether it survives the mobile crop. If it does not, use copy above/below the media on mobile. A quiet dark background is not proof of sufficient contrast: check in the consuming page.

## Copyable prompts

Start prompt: state intended page location and aspect; describe the concrete scene, materials, lighting, lens, framing, negative space, source-image roles and explicit fidelity constraints. Avoid promotional slogans and unsupported facts. Include no text/logo if reliable raster lettering is not essential; an existing logo can be added later as a web layer.

End prompt: explicitly say “Use the generated START image as the primary image reference.” Repeat the concrete scene and all fixed anchors so the prompt remains usable on its own. Change only the planned motion. Keep subject count, construction and illumination. Do not introduce a new composition.

Video prompt: identify START and END inputs; repeat the scene; give a short timing plan, e.g. 0–0.5s hold, 0.5–4.5s small eased movement, 4.5–5s settle. Specify what remains fixed. No dissolve between two photographs as a substitute for coherent motion. No sound, hard cuts or loop promise unless explicitly justified. If a target generator cannot support both endpoints, write a self-contained single-image video prompt that uses START only and describes the desired end state explicitly. Do not tell the user to paste a two-image prompt that still refers to an unavailable “supplied END”. Explain that the described end state is a guide, not an enforced last frame. If endpoint support is unknown, keep recommendations conditional and do not invent a provider's settings.

When actual generated dimensions differ from the requested ratio, report the actual ratio and choose an appropriate fit/export treatment. Never stretch or promise a lossless portrait crop. Copy-space measurements refer to the observed result, not the prompt's requested percentages. In prompt-only mode crop and continuity claims remain design intentions, not checked image facts.

## Media delivery advice

Suggested duration and frame rate are production recommendations, not an invented provider API. A 5-second, 24–30fps source is often adequate; site purpose decides. Choose a master with enough resolution for the placement and a smaller mobile derivative after actual export inspection. Use a lightweight poster and compressed web delivery. Do not set a universal byte target, autoplay policy or hardware-performance promise. Scroll films must be tested on actual visual output in both directions; reduced-motion can remain a still. Default distinct endpoints should play once or be scroll-controlled, not looped with a visible jump.
