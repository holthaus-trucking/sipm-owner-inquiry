# SI Property Management — Owner Inquiry Form

Public owner inquiry form for SI Property Management. Submissions are emailed to `owner@sirentnow.com` through Form.taxi (`https://form.taxi/s/ukz5915a`).

## Live URLs

- Form: https://sipm-owner-inquiry.onrender.com/
- Full-management ad: https://sipm-owner-inquiry.onrender.com/?ad=full
- Placement special ad: https://sipm-owner-inquiry.onrender.com/?ad=placement
- Thank-you page: https://sipm-owner-inquiry.onrender.com/thanks.html

Leads are emailed to `owner@sirentnow.com` with subject `New SIPM Owner Lead`. The Form.taxi account email does not need a separate activation click. Hidden fields set `_next` to the thank-you page, `_replyto` to the visitor's email, and `_gotcha` as a honeypot.

## Form fields

Full name, email, and phone are always required, plus a required dropdown: **What type of property do you own?**

1. **Single-family residential** — property address (required), size (sq ft), bedrooms, bathrooms.
2. **Multifamily only** and **Combination of both** (multifamily and single-family) share the same fields: property address(es) (required), total number of units/doors (required), and town(s) or county(ies) (optional). The only difference is the `property_type` value from the dropdown.

Only the visible section's fields are submitted. A hidden `source` field records `placement`, `full`, or `direct` from the `?ad=` query param.

## Redeploy

This is a Render static site (`sipm-owner-inquiry`) in the Holthaus Render workspace, published from the `public/` folder on the `main` branch of this repo.

1. Edit files in `public/` (`index.html`, `thanks.html`, `logo.png`).
2. Commit and push to `main`.
3. Auto-deploy is on, so Render will rebuild and publish. There is no build step (`buildCommand` is `true`); `publishPath` is `public`.

Manual deploy: Render Dashboard → sipm-owner-inquiry → Manual Deploy, or the Render `trigger_deploy` MCP tool.

Source of truth used to build this page also lives on the agent box at `/workspace/sipm_ad/inquiry_form/`.
