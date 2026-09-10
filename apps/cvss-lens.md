# CVSS Lens

Source: [cvss-lens](https://github.com/offware-apps/cvss-lens), `README.md` at 4d0a2ed, the section copied verbatim. The repository's file wins where this copy has drifted.

## The vector never leaves the browser

It lives in the URL fragment, after the `#`, which browsers do not send to the
server. A vector for an embargoed finding therefore reaches nobody, the host
serving the page included. A `?vector=` version would put it in the request line
and in every log along the way, which is why the fragment is the one design
constraint the page cannot trade away.

One file. No CDN, no web font, no analytics, no request of any kind:
[`test/cvss.test.mjs`](https://github.com/offware-apps/cvss-lens/blob/main/test/cvss.test.mjs)
fails on a `src`, a stylesheet link, a `fetch` or an `XMLHttpRequest`
appearing in
[`index.html`](https://github.com/offware-apps/cvss-lens/blob/main/index.html).

