# GrandLime Labs waitlist

Static waitlist page for **GrandLime Labs** (*Plot A Course For Greatness*), a small studio making digital products: illustrated books and software tools.

Free email signup only: no prices, preorders, payments, or donations. There is no business licence until January 2027.

Live site: https://grandlime-labs.github.io/waitlist/

## Form

The page is plain HTML/CSS and works without JavaScript. The form `POST`s to Buttondown’s public embed endpoint (no API keys or other secrets in the client):

`https://buttondown.com/api/emails/embed-subscribe/grandlimelabs`

The only field is a required email input, `name="email"`. Do not submit this form with `fetch()`: Buttondown may need the browser to follow the response for a CAPTCHA or validation page.

The privacy line on the page is: we use your email only for launch updates, and you can unsubscribe anytime.

## Files

- `index.html`, `style.css` — page and brand styles (navy `#0E1633`, lime `#9DD300`, Lilita One + Lato)
- `assets/logo.png` — GrandLime Labs mark
- `assets/fonts/` — self-hosted Lato and Lilita One (SIL Open Font License; OFL text files are in that folder)
- `.github/workflows/pages.yml` — deploys the static files to GitHub Pages

The book teaser uses only wording already approved for *Sixteen Milliseconds*: the title, the subtitle “How GPUs and Game Engines Build Your Game,” and “Coming 2027.”

## License

MIT. See `LICENSE`.
