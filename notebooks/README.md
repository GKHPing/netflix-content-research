## 1. Research Motivation

Using publicly available catalogue metadata, this analysis examines how Netflix’s content strategy
has evolved along two dimensions:

1. The balance between regional distribution of content regardless of movies and TV series over time.
2. The extent to which different genres are regionally distributed.

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
- Limit up to 50 pages for each Movies and TV shows as it called via API not a entire data dump to consume

## 2. Pull data from TMDB via API

- NETFLIX_PROVIDER_ID = 8   
- regions = ["SG","MY","ID","PH","TH","VN","BN","AU","NZ","TW","HK"]

## 3. Data Cleaning

- Parse dates and basic cleaning of genre and data added estimate fields
- Limit data to 2025
- Deduplicate titles


