# Paper reader

One web page (`index.html`) that turns the LaTeX source of a paper into a single reading file:
every reference opens its target in place, every symbol in a formula shows where it is defined,
and every proof gets an outline of its steps written by Claude.

- It runs in your browser; this site has no server. Drop a .zip or .tar.gz of the sources. The
  page converts the paper locally and shows the estimated cost of the model stages. Nothing is
  sent until you press Generate. Then the paper goes from your browser to Anthropic's API, under
  your own API key.
- Without a key it still builds a reader with clickable references and automatically found
  notation, at no cost.
- The key is kept in your browser's local storage for this site (untick "Remember the key" to
  avoid that) and is never written into a reader. Use a key made for this, in a Claude Console
  workspace with a monthly spend limit.
- Proof outlines are written by a model and marked "machine-written, not checked".
- The page loads fonts from Google Fonts, and pdf.js from cdnjs when a paper has PDF figures.

`index.html` is a build; its source is not published here.
