# X Publishing Workflow

Use this when the user wants posts uploaded or published to X.

## Default Behavior

- If the user only asks for drafts, do not open X.
- If the user says publish, upload, post, automate, or send to X, open the browser and continue.
- Publish only the posts the user explicitly asked for, except that automation phrases mean publish the full 5-post batch.
- Prefer the already logged-in desktop Chrome session if it is available and stable.
- Keep the publish path simple: do not clone browser profiles, rebuild sessions, or depend on extension bridges when the logged-in X window is already available.

## Browser Flow

1. Open `https://x.com/compose/post`.
2. If login is required, stop and ask the user to sign in in the browser.
3. Paste the post copy exactly.
4. If the post has a local image file path, attach the image before publishing.
5. Confirm the text matches the intended draft, without extra claims or placeholders.
6. Confirm the image preview is visible when an image is attached.
7. For a thread, add the next post using the composer plus flow.
8. Review for truncation, broken line breaks, and accidental extra text.
9. Publish only after the user has explicitly asked to publish in the current request.
10. If the existing logged-in browser is already on X, use that window directly instead of switching tools or profiles.

## 5-Post Batch Flow

Use this when the user asks for one-shot automation or publishing all 5 posts.

1. Generate exactly 5 posts before opening X.
2. Keep the 5 posts in order and do not remix them while publishing.
3. If images are provided, keep the image order aligned with the post order.
4. Open `https://x.com/compose/post`.
5. Paste Post 01, attach Image 01 if available, review, publish, and confirm the sent state.
6. Repeat the same compose-review-publish-confirm loop for Post 02 through Post 05.
7. If X blocks, rate-limits, shows an error, or the composer is not stable, stop immediately.
8. Report sent and unsent posts separately.

## Safety Checks

- Never add claims that were not in the draft.
- Never add hashtags, links, or mentions unless the draft includes them or the user asked for them.
- Never publish a draft that contains placeholders.
- If multiple drafts are prepared, ask which ones to publish unless the user clearly asked for all 5 or used a batch automation phrase.
- If an image is attached, make sure it matches the intended post before sending.

## Suggested Execution Order

1. Generate the copy package.
2. Select the exact posts to publish; for automation, select all 5.
3. Open X in the browser.
4. Compose and review each post.
5. Publish.
6. Confirm the sent state.
7. Report success.
