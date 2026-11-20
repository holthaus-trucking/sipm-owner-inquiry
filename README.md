# SI Property Management — Owner Inquiry Form

Public owner inquiry form for SI Property Management. Submissions are emailed to `owner@sirentnow.com` through FormSubmit.

## Live URLs

- Form: https://sipm-owner-inquiry.onrender.com/
- Full-management ad: https://sipm-owner-inquiry.onrender.com/?ad=full
- Placement special ad: https://sipm-owner-inquiry.onrender.com/?ad=placement
- Thank-you page: https://sipm-owner-inquiry.onrender.com/thanks.html

The first real submission sends an activation email to `owner@sirentnow.com`. Someone must click the confirmation link before leads will arrive.

## Redeploy

This is a Render static site (`sipm-owner-inquiry`) in the Holthaus Render workspace, published from the `public/` folder on the `main` branch of this repo.

1. Edit files in `public/` (`index.html`, `thanks.html`, `logo.png`).
2. Commit and push to `main`.
3. Auto-deploy is on, so Render will rebuild and publish. There is no build step (`buildCommand` is `true`); `publishPath` is `public`.

Manual deploy: Render Dashboard → sipm-owner-inquiry → Manual Deploy, or the Render `trigger_deploy` MCP tool.

Source of truth used to build this page also lives on the agent box at `/workspace/sipm_ad/inquiry_form/`.
