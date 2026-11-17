# RAN-NEETI — Full Feature Streamlit Build

This build implements the workflows described in the RAN-NEETI project report:
- Home Dashboard
- Real Sports Lab with sport, format, venue, two competitors, competition/date, context and advanced instructions
- Anime & Fictional Battles with matchup type, universe, character versions/story arcs and scenario rules
- MediaWiki entity lookup for sports/general entities
- Jikan character lookup with MediaWiki fallback
- Gemini API analysis with Google Search grounding and extracted source links
- Structured report sections: evidence, outcome estimates, strengths/weaknesses, major moves, counters, turning points, win conditions, outcome paths and uncertainty
- Recent Reports session history
- Markdown downloads
- About RAN-NEETI project page
- API connection test and input/error handling

## Deploy without installing Python locally
1. Extract the ZIP.
2. Upload the *contents* of this folder to the root of a GitHub repository.
3. On Streamlit Community Cloud, create an app from that repository and set the main file path to `app.py`.
4. In App settings → Secrets, add:

```toml
GEMINI_API_KEY = "YOUR_PRIVATE_GEMINI_API_KEY"
GEMINI_MODEL = "gemini-3.8-flash"
```

5. Save, reboot the app, and use **TEST API CONNECTION** in the sidebar.

Never put the API key in source code, GitHub, screenshots, or chat.

## Important academic limitation
This is a search-grounded AI research/reporting application. It does not contain trained sport-specific ML models, historical model-training pipelines, calibrated probability forecasts, or validated accuracy metrics. Sports percentages must be presented as qualitative AI estimates. Fictional matchup percentages are subjective scenario interpretations.

## Runtime verification
Python syntax compilation can be checked locally, but live operation requires Streamlit, internet access, a valid Gemini API key, model access and quota. Public API responses and deployment must be tested in the deployed environment.
