# RepayPal

A free, single-page repayment estimator for revenue-based financing (merchant cash advance) borrowers. It shows total repayment, payment size, payoff time, estimated APR and share of sales, all calculated in the browser.

## Files

- `index.html`: the complete tool (HTML, CSS and JavaScript in one file, no dependencies)
- `README.md`: this file

## Run locally

Open `index.html` in any browser. No build step or server is needed.

## Publish with GitHub Pages

1. Create a new repository on GitHub (for example, `repaypal`).
2. Upload `index.html` and `README.md` to the repository root.
3. Go to **Settings > Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose the `main` branch and the `/ (root)` folder, then save.
5. After a minute or two, the tool is live at `https://<your-username>.github.io/<repository-name>/`.

## Customize

Edit the values near the top of `index.html`:

- Slider ranges: the `min`, `max` and `step` attributes on the inputs (advance amount, factor rate, fee, term, share of sales).
- Default values: the `value` attributes on the same inputs.
- Quick-start examples: the `data-a` (amount) and `data-s` (monthly sales) attributes on the `.chip` buttons.
- Payment days per month: `ppm` and `ppy` inside the `run()` function (currently 21 per month and 252 per year for daily payments).
- Contact form: the "Send my estimate" button currently shows a thank-you message only. Nothing is sent or stored. Connect it to your CRM or a form service before real use.

## Important

This tool provides estimates only. It is not an offer, approval or commitment to lend. Some states require specific disclosures for commercial financing, including APR, so have legal counsel review the wording and calculations before using it with real borrowers.
