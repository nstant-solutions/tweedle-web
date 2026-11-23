# tweedle-web

The Tweedle website, served by GitHub Pages from `main`:
https://nstant-solutions.github.io/tweedle-web/

- `privacy/` is the privacy policy linked from both store listings. Its source is
  `docs/privacy_policy.md` in the game repo. After changing that file, rebuild the body:

  ```sh
  gh api /markdown -f mode=markdown -F text=@../tweedle/docs/privacy_policy.md
  ```

  and replace everything inside `<main>` in `privacy/index.html` with the output.
