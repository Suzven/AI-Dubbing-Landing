DUBLIFT LANDING — Cloudflare Pages deployment
=============================================

1) Deploy (no build step needed, pure static HTML):
   - Go to Cloudflare Dashboard -> Workers & Pages -> Create -> Pages
   - Choose "Upload assets" (Direct Upload)
   - Drag this ZIP (or the extracted folder) into the upload area
   - Name the project -> Deploy. Done: you get https://<project>.pages.dev

2) BEFORE LAUNCH — replace 2 things:
   a) Email: search for "hello@dublift.example" in index.html (2 places:
      footer + the <script> at the bottom) and put your real email.
   b) Brand name "Dublift" if you want a different one.

3) Form / funnel note:
   The form currently opens the visitor's email client with a pre-filled
   message (works with zero backend). For silent lead capture, create a
   free form at formspree.io or tally.so and replace the <script> handler
   with a normal POST — takes ~5 minutes.

4) Analytics for niche validation:
   Add Cloudflare Web Analytics (free, one <script> tag, no cookies):
   Dashboard -> Analytics & Logs -> Web Analytics -> Add site,
   paste the snippet before </body>.

v4 personalization checklist:
- Replace "Andrii" (founder note + form note) with the real founder name.
- The reviewer names in "The human part" block (Marta, Jonas, Olha) are
  illustrative — swap in your real reviewers' first names as you hire them.
- Production ticket #0007 is an example; update details after first real jobs.

v17 form delivery:
- Submissions are emailed via FormSubmit to killagroup22@gmail.com with a CC
  to suzven9@gmail.com. No account or backend needed.
- IMPORTANT one-time step: after deploying, submit the form once yourself.
  FormSubmit will send an activation email to killagroup22@gmail.com —
  click "Activate" in it. From then on all submissions arrive automatically.
- If the network request ever fails, the page falls back to opening the
  visitor's mail app addressed to both inboxes, plus a copyable text block.
