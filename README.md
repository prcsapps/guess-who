# Guess Who?

A single-page mobile game. Upload photos of friends and family, crop three levels on each photo (hardest to easiest), then guess who it is by typing the name.

- Photos stay in the browser on your own device (IndexedDB). Nothing is uploaded anywhere.
- Open `index.html` in a browser, or host the folder with GitHub Pages.

## Run it

Open `index.html`, or serve the folder:

```
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Host it on GitHub Pages

1. Push these files to a GitHub repository.
2. In the repository, go to Settings, then Pages.
3. Under Build and deployment, choose Deploy from a branch, pick `main` and `/ (root)`, and save.
4. Your game will be at `https://<your-username>.github.io/<repo-name>/`.
