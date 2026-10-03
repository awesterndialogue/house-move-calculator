# Next Home Calculator

A single-file GitHub Pages calculator for modeling when a move from Lakewood becomes affordable.

## Main levers

- New home price
- Mortgage interest rate
- Years we stay at Lakewood
- 15-year vs. 30-year mortgage
- All-in monthly payment ceiling

## How the Lakewood projection works

The site keeps the Lakewood sale value **flat** until you manually update it. This is intentional: there is no assumed home appreciation.

In **Advanced assumptions**, enter:

- Current Lakewood sale value after your realtor / fix-up allowance, but before mortgage payoff
- Current Lakewood mortgage balance
- Lakewood mortgage interest rate
- Current monthly principal + interest payment

The “Years we stay at Lakewood” slider amortizes the current mortgage forward using those inputs and subtracts the projected future mortgage balance from the stored Lakewood sale value. That produces the estimated proceeds available for the next purchase.

All values are saved in the browser with localStorage. Shareable scenario links also include the assumptions in the URL.

## Publish on GitHub Pages

1. Create a GitHub repository.
2. Upload `index.html` to the repository root.
3. In GitHub, open **Settings → Pages**.
4. Set the source to **Deploy from a branch**.
5. Select the main branch and `/ (root)`.
6. Save. GitHub will provide the public URL.

No Firebase, build process, framework, or server is required.
