# Tamon Fukuhara — ComfyUI Prompts

## Style Lock
Base: _AnimeBoy
Checkpoint: illustrious\Illustrious-XL-v2.0.safetensors
LoRAs: illustriousXL_stabilizer_v1.93 (0.5), Eyes_for_Illustrious_Lora_Perfect_anime_eyes (0.6), bemen-000009 (0.8), Z-image\CHATGPT (0.75)
Resolution: 1024×1360
Steps / CFG / Sampler / Scheduler: 25 / 7 / dpmpp_2m_sde / karras
Denoise: 0.8

---

## Shared Negative Prompt

```
worst quality, low quality, bad anatomy, bad hands, extra fingers, missing fingers,
extra limbs, deformed, blurry face, watermark, text, cropped,
1girl, female, feminine, girl, woman,
beard, stubble, mustache,
old, aged, mature, wrinkled,
nude, nipples, exposed_chest, shirtless, nsfw, lewd, suggestive_pose
```

---

## Shot 1 — Off-Duty / Gloomyhara
*Upper body portrait, dim apartment, mid-spiral energy. The real one.*

```
masterpiece, best quality, newest, absurdres, highres, very aesthetic,
1boy, solo, male_focus, looking_at_viewer, upper_body,
18_years_old, young_man, lean_build,
pink_hair, messy_hair, disheveled_hair, pink_eyebrows, grey_eyes,
parted_lips, tired_expression, melancholic, vacant_gaze, dark_circles,
black_hoodie, oversized_clothes, long_sleeves, hood_down,
lying_on_couch, indoors, dim_lighting, single_lamp, curtains_closed,
shadow, dark_room, atmospheric, moody, low_key_lighting
```

---

## Shot 2 — Hottiehara
*Upper body, styled and performing. The packaged version.*

```
masterpiece, best quality, newest, absurdres, highres, very aesthetic,
1boy, solo, male_focus, looking_at_viewer, upper_body,
18_years_old, young_man, lean_build,
pink_hair, swept_bangs, side_part, styled_hair, pink_eyebrows, grey_eyes,
smirk, confident_expression, charismatic, slight_smile,
jacket, open_collar, idol_outfit, dark_clothing,
dramatic_lighting, spotlight, dark_background, rim_light,
sharp, vivid, stage_lighting
```

---

## Shot 3 — Darkhara
*Close-up / face focus, very still, watching. The possessive one.*

```
masterpiece, best quality, newest, absurdres, highres, very aesthetic,
1boy, solo, male_focus, looking_at_viewer, close-up, face_focus,
18_years_old, young_man, lean_build,
pink_hair, messy_hair, pink_eyebrows, grey_eyes,
serious_expression, cold_expression, intense_gaze, blank_stare,
black_hoodie, long_sleeves,
flat_lighting, neutral_background, high_contrast, hard_shadow,
stillness, controlled, quiet_menace
```

---

## Notes
- All three shots are clothed reference portraits — nudity negatives are in the shared block.
- Shot 1 and 3 use the same off-duty outfit (black hoodie); only Shot 2 swaps to an idol look.
- Darkhara reads best as a tight crop — face_focus with minimal background is intentional.
- If Shot 2 drifts toward generic idol rather than specifically Tamon, pull back on `charismatic`
  and lean harder on the pink_hair / grey_eyes anchors; his look is distinctive enough to carry it.
- First-pass these at _AnimeBoy's default denoise (0.8). If the face softens too much,
  let FaceDetailer do the work rather than bumping denoise — that's what it's there for.
