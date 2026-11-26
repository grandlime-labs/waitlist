# GrandLime Labs waitlist

Static waitlist page for **GrandLime Labs** (*Plot A Course For Greatness*), the digital-products division of GrandLime.

Free email signup only: no prices, preorders, payments, or donations. There is no business licence until January 2027.

Live site: https://grandlime-labs.github.io/waitlist/

## Form

The page is plain HTML/CSS and works without JavaScript. The form `POST`s to Buttondown’s public embed endpoint (no API keys or other secrets in the client):

`https://buttondown.com/api/emails/embed-subscribe/grandlimelabs`

| Field | HTML `name` / `value` |
| --- | --- |
| Email (required) | `name="email"` |
| Book (optional) | `name="tag"` `value="book"` |
| Software tools (optional) | `name="tag"` `value="software-tools"` |

Interest checkboxes use Buttondown’s documented embed-form `tag` inputs. Buttondown auto-creates a tag if it does not already exist, so the tags do not have to be created in the dashboard first. **Tagging & segmentation is a paid Buttondown add-on** (not part of the free plan). Email signup itself works on the free plan; interest tags may only apply once that add-on is enabled. Do not submit this form with `fetch()`: Buttondown may need the browser to follow the response for a CAPTCHA or validation page.

The privacy line on the page is: we use your email only for launch updates, and you can unsubscribe anytime.

## Files

- `index.html`, `style.css` — page and brand styles (navy `#0E1633`, lime `#9DD300`, Lilita One + Lato)
- `assets/logo.png` — GrandLime Labs mark
- `assets/fonts/` — self-hosted Lato and Lilita One (SIL Open Font License; OFL text files are in that folder)
- `.github/workflows/pages.yml` — deploys the static files to GitHub Pages

The book teaser uses only wording already approved for *Sixteen Milliseconds*: the title, the subtitle “How GPUs and Game Engines Build Your Game,” and “Coming 2027.”

## License

MIT. See `LICENSE`.
