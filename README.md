# PokéScan

PokéScan is a single-file Pokémon trading card scanner/search app.

## Publish with GitHub Pages

1. Create a new GitHub repository named `pokescan`.
2. Set it to **Public**.
3. Upload `index.html` from this folder to the repository root.
4. Open the repository's **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch **main** and folder **/(root)**, then save.
7. Wait for the Pages URL to appear. It will usually look like:
   `https://YOUR-USERNAME.github.io/pokescan/`

## Notes

- The app calls TCGdex directly for public card data.
- AI identification uses the PokéScan Supabase Edge Function. Keep the Groq API key in Supabase secrets; never put it in this HTML file.
- This is a public website. Anyone can visit it, so keep backend rate limits enabled.
- The collection is stored in the visitor's browser (localStorage), so it does not automatically sync across devices.
