## 1. Research Motivation

Using publicly available catalogue metadata, this analysis examines how Netflix’s content strategy
has evolved along three dimensions:

1. The balance between movies and series over time.
2. The extent to which different genres are regionally distributed.
3. How localisation varies across major regional markets.

This analysis is descriptive rather than causal and focuses on supply-side strategy rather than user behaviour.

## 2. Data Overview & Limitations

The dataset consists of Netflix movie and TV show catalogue metadata up to 2025.
Each row represents a title made available on the platform.

Key fields used:
- `type`: Movie or TV Show
- `genres`: Genre classifications
- `regions`: Country region associated with the title
- `date_added_estimated`: Date the title was added to Netflix

Limitations:
- No viewership or engagement data
- Multi-country entries complicate regional attribution

## 2. Pull data from TMDB via API

-NETFLIX_PROVIDER_ID = 8    # TMDB provider ID for Netflix
-regions = ["SG","MY","ID","PH","TH","VN","BN","AU","NZ","TW","HK"]

## 3. Data Cleaning

-Parse dates and basic cleaning of genre and data added estimate fields
-Limit data to 2025
-Deduplicate titles


## 5. Analysis & Findings

1) How has Netflix’s content mix (movies vs series) evolved over time?
The results show a clear shift in Netflix’s catalogue composition over time,
with TV series representing an increasing share of newly added titles,
consistent with a strategy focused on subscriber retention and episodic engagement.

2) Which genres appear most regionally distributed?
Genres such as International Dramas and Documentaries exhibit broader geographic
distribution, suggesting higher portability across markets.
Conversely, culturally specific genres tend to have narrower distribution.

3) How does regional localisation vary across markets?
Markets such as the United States exhibit lower concentration, reflecting a more
globally diverse catalogue. In contrast, markets like India and South Korea show
higher localisation, consistent with strong domestic production ecosystems.


## 6. Next Steps

With access to internal data, future research could:
- Link catalogue composition to subscriber retention outcomes
- Distinguish production origin from distribution markets

