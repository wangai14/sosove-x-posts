---
name: sosove-x-posts
description: Generate and batch-publish 5 daily Japanese X post drafts for SOSOVE, the fashion site at sosove.com. Use when the user asks to write, batch, automate, refresh, schedule, upload, publish, or prepare image prompts for SOSOVE social posts, especially a simple 5-post compose-and-post flow with sharp seasonal controversy, current Japan lifestyle hooks, purchase desire, optional image-generation prompts, and optional user-provided images sent directly through the currently logged-in X browser.
---

# SOSOVE X Posts

## Purpose

Create daily Japanese X post copy for SOSOVE as a 5-post batch. When the user needs images generated first, provide one image-generation prompt per post. When the user provides 5 images, match each caption to the corresponding image in order. When the user explicitly asks to publish, automate, or batch-post, use the currently logged-in X browser window directly and keep the flow minimal: open compose, paste copy, attach image, post, verify. Do not rely on copied Chrome profiles, browser-bridge reconstruction, or other session-rebuild tricks.

Use the house baseline in `references/sosove-x-style.md` and the seasonal trigger map in `references/seasonal-event-hooks.md` unless the user gives newer direction. If a post depends on current products, prices, discounts, stock, materials, holidays, weather, news, or trend details, verify the current source before writing; otherwise keep the hook general.

## Daily Workflow

1. Pick the day angle.
   - Monday: white denim and light colors.
   - Tuesday: denim shirt and easy layering.
   - Wednesday: skirts and not-too-sweet adult femininity.
   - Thursday: wide pants, suspenders, silhouette, and comfort.
   - Friday: cheap-looking vs polished basics.
   - Saturday: trend critique and contrast hooks.
   - Sunday: soft brand mood and reset-the-closet ideas.
2. Pick one current seasonal or lifestyle trigger from the reference, such as heat, rain, humidity, commute, vacation prep, payday, bonus season, school event, office AC, or wardrobe reset.
3. Pick 2-3 tension points from the style reference.
4. Write in Japanese, short lines, X-native rhythm, strong first line.
5. Make the reader feel "this is my current problem" before mentioning SOSOVE.
6. Keep controversy focused on clothing choices, styling habits, and common assumptions.
7. End with a soft purchase nudge only when useful.

## Default Output

When the user asks for today's SOSOVE posts, output:

- 5 single-post drafts.
- 2 comment CTAs.
- 3 hook-only ideas.
- A short Chinese note with assumptions if the live site was not checked.

For each single post, keep it roughly 70-180 Japanese characters.

Use this compact format:

```text
Post 01
Image:
Copy:
Seasonal trigger:
Controversy:
Comment CTA:
Status:
```

Do not output a mini thread unless the user asks for one.

## Image Prompt Preparation Mode

If the user asks for image prompts, image generation prompts, picture prompts, "generate image first", or similar:

1. Generate exactly 5 post packages.
2. For each package, include the Japanese copy, an English image prompt, suggested aspect ratio, overlay text if useful, and a short visual note.
3. Make each image prompt correspond directly to the post copy.
4. Keep images editorial, fashion-focused, and compatible with SOSOVE's adult casual style.
5. Do not imply the generated image is an exact product photo unless the user provided the exact product image or source page.
6. Prefer 16:9 when the image includes text overlay; prefer 4:5 when the image is an outfit photo.

Use this format:

```text
Post 01
Copy:
Image prompt:
Aspect:
Overlay text:
Visual note:
Publish status:
```

## Provided Image Batch Mode

If the user provides 5 images:

1. Treat the images as ordered: Image 01 maps to Post 01, Image 02 maps to Post 02, and so on.
2. Analyze the visible outfit, item, color, text overlay, season, and purchase angle in each image.
3. Write copy that complements the image; do not simply repeat text already visible in the image unless repetition improves the hook.
4. Keep the caption short enough that the image remains the main scroll-stopper.
5. If the images are attached in chat but no local file paths are available, generate the 5 captions but ask for local file paths before automated X upload.
6. If local image file paths are available, publish each post with its matching image attachment.

## Batch Automation Mode

If the user asks for automation, one-shot posting, all 5 posts, or batch publishing:

1. Generate exactly 5 publish-ready posts.
2. If images are provided, pair each post with the image in the same order.
3. Treat the batch as the selected publish set.
4. Publish posts in order: Post 01, Post 02, Post 03, Post 04, Post 05.
5. After each publish, confirm the sent state before composing the next post.
6. If one post fails, stop and report which posts were already sent and which remain.
7. After publishing all 5, report the exact 5 texts and image names or paths that were sent.
8. Use the same logged-in X browser window for the full batch; do not rebuild browser state or switch to a copied profile.

## Voice Rules

- Lead with a blunt but defensible opinion.
- Tie the opinion to the current season, weather, or daily life moment whenever possible.
- Sound like a sharp fashion observer, not a brand account.
- Use simple Japanese.
- Use line breaks for rhythm.
- Mention SOSOVE sparingly.
- Prefer soft site nudges over hard sales copy.
- Write for resonance first, desire second, brand third.

## Truth And Safety Rules

- Do not invent customer reviews, purchase experiences, before/after results, rankings, sellout claims, discounts, urgency, or numeric proof.
- Do not write as if the poster personally bought or wore the item unless the user explicitly provides that experience.
- Do not claim a material, fabric function, stain resistance, waterproofing, stock status, shipping detail, or sale price unless verified on the current site.
- Avoid direct age or body insults. Critique the styling outcome instead.
- Avoid defamatory or comparative claims about named competitors.

## Publishing Mode

If the user says to publish, upload, post, automate, or send to X:

1. Generate the selected post copy first.
2. Use the existing logged-in X browser window when available; prefer the browser surface that is already open and signed in.
3. Open the X compose flow directly in that browser.
4. Paste the exact copy.
5. If the post has an image, attach the matching image before publishing and verify the preview is visible.
6. Verify the composer contains only the intended copy and the Post button is active.
7. If the user asked for automation or a 5-post batch, publish all 5 in order. Otherwise publish only the posts the user asked to publish.
8. Confirm each post was sent, then report which posts were published and keep the rest as drafts.
9. If the browser opens to a login page or the compose flow is not available, stop and ask the user to sign in in that browser, then continue from there.

## Product-Specific Requests

If the user gives a product URL, product name, campaign, or screenshot:

1. Extract the exact product facts first.
2. Build 5-8 posts around one objection and one styling benefit.
3. Include 2 softer variants if the first drafts are too aggressive.
4. Note any facts that should be checked before publishing.

## References

Read `references/sosove-x-style.md` for brand tone and content angles.
Read `references/seasonal-event-hooks.md` when generating daily posts, especially if the user asks for current-season controversy or purchase desire.
Read `references/x-publishing-workflow.md` when the user asks to publish or upload posts in the browser.
