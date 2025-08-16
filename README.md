# Personal Movie Collection (Google Sheets)

**What it is**
- A private tool to catalog physical movies I own.
- Uses Google Sheets + Apps Script to:
  - auto-pick **one** genre from my controlled list (Column C) using ChatGPT
  - fetch and display a movie’s theatrical poster (Column D) from **TMDB**

**How it works**
- I type a title in **Column A**.
- Apps Script calls:
  - OpenAI Chat Completions to choose one genre from `Lists!A:A`
  - TMDB Search API for the poster and inserts it with `=IMAGE()`
- API keys are stored in **Script properties** (not in code).
- No server or database; single-user, non-commercial.

**APIs**
- OpenAI (ChatGPT) for single-label genre classification.
- The Movie Database (TMDB) for poster lookup.
- *This product uses the TMDB API but is not endorsed by TMDB.*

**Privacy**
- No user accounts. No analytics. No data resale.
- Only movie titles are sent to the APIs as needed.

**Status**
- Personal/desktop use only. Non-commercial.

**Contact**
- Open a GitHub issue in this repo.
