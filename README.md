# Free Secret Santa generator (one HTML file, nothing stored)

A Secret Santa name draw that runs entirely in the browser. Type the names, tap **Draw names**, then send each person their own private link on WhatsApp, text, email or the share sheet. Each link reveals only that person's match.

**Use it now, no install:** [tchworks.co.uk/free/secret-santa-generator](https://www.tchworks.co.uk/free/secret-santa-generator/?utm_source=github&utm_campaign=ss-repo)

## What it does

- Nobody draws themselves.
- **Keep apart** pairs (couples, flatmates), one pair per line, e.g. `Mum & Dad`.
- Clear errors for duplicate names, unknown keep-apart names and rules that make a fair draw impossible.
- Optional group name, spend limit and swap date, shown on each reveal.
- Uses `crypto.getRandomValues` for the shuffle.
- Handles accented names (Zoë, Siân, Seán).

## Privacy

There is no server. The draw happens in the organiser's browser, and each person's match is stored only inside the `#r=` fragment of their own link. URL fragments are not sent to the web server when the link is opened. Nothing is saved or collected.

The fragment is lightly scrambled so a match isn't readable at a glance. It is **not** encryption: anyone who decodes a link on purpose can see that one match. That's fine for office and family Secret Santa, but don't use it for anything that needs real secrecy.

## Self-host

It's a single file with no dependencies or build step. Put `index.html` on any static host (GitHub Pages, Netlify, an intranet share, a WordPress media upload) and the reveal links point back to wherever you host it.

## Tips that save arguments

- Pick one spend limit. £10 is the common UK office middle ground; £5 suits big teams and £20 to £30 families.
- Draw by mid-November so people can order online without paying for fast delivery.
- Ask for a three-item wish list: one practical, one fun, one food or drink.
- Agree the swap date before the draw.

## Printables

For sign-up sheets, a rules and budget poster, name-draw slips, wish list cards and gift tags, there's the [Secret Santa Organiser Kit](https://www.tchworks.co.uk/shop/secret-santa-organiser-kit?utm_source=github&utm_campaign=ss-repo) (£2.49, print at home).

## Licence

MIT. Made by [TCH Works](https://www.tchworks.co.uk/?utm_source=github&utm_campaign=ss-repo).
