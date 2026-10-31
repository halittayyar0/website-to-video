# Result structure

Use actual decisions and source URLs; replace these field descriptions rather than returning placeholders.

Before this result, resolve the Codex output-mode question if needed; an unanswered choice is not a completed result. Once selected, name the mode briefly without repeating the question.

1. **Site and concept:** 3–5 sentences in the user's language. Offer, audience, CTA, selected page placement and why this scene serves it. Separate verified facts from illustrative direction. Add a compact source ledger with access limitations, including the actual image/reference inspected.
2. **START:** the generated image and saved path, or a complete English image prompt in its own copyable block. If generated, include the prompt too for reproducibility.
3. **END:** the generated image and saved path, or a complete English prompt in its own block. State which actual START image was attached. If prompt-only, give the explicit attach-START instruction inside the prompt.
4. **VIDEO PROMPT:** one complete English block compatible with the selected target. Include scene, input roles, timing, motion, camera, invariants, and negatives. If the target accepts only START, make the delivered video prompt START-only and describe the end state in prose; omit an unusable dual-input version unless the user asks for both. If target capability is unknown, keep a tool-neutral dual-endpoint prompt conditional on verified support, without inventing parameters. Explain any weaker endpoint constraint outside the copyable block.
5. **Use settings:** placement, duration, requested and actual master aspect, crop-safe region, HTML copy location, audio, poster, motion/accessibility fallback, once/scroll behavior. State the actual asset status and whether any video has been generated or tested. If a pair failed, list its defect and pending stage; do not label it accepted or silently switch to prompts. Keep the checked limitation short and specific.

Do not pad the response with multiple competing concepts or a questionnaire. Exactly two endpoint assets; do not count contact sheets, discarded attempts or an optional poster as extra endpoints.
