# Consumer Insights for Beats by Dre

**Author:** Musa Nofisat Bolanle  
**Project type:** Consumer insights, exploratory data analysis, NLP and sentiment analysis  
**Notebook:** `notebooks/Beats_by_Dre_Consumer_Insights_Capstone_Project.ipynb`

## Project Overview

This capstone project analyzes customer reviews of Beats by Dre's portable speaker products and competing products. The aim is to understand customer satisfaction, identify recurring themes in review text, compare sentiment across products, and translate review evidence into product and marketing recommendations.

## Objectives

- Explore customer ratings and review patterns.
- Clean and prepare review data for analysis.
- Analyze review text using TextBlob and NLTK VADER sentiment methods.
- Visualize rating distributions, review timelines, and common review terms.
- Use Gemini AI to summarize themes in a subset of customer reviews.
- Compare Beats Pill with competing portable speaker products.
- Develop evidence-informed product and marketing recommendations.

## Dataset

The notebook describes data collected from Amazon product reviews using Oxylabs, then combined into a CSV for analysis. The analysis includes review text, ratings, product identifiers, timestamps, and product attributes.

The notebook's cleaning output shows **1,122 rows before cleaning and 1,022 rows in the later cleaned dataframe**. The written descriptive-statistics section also reports 952 reviews, so these counts should be reconciled against the final dataset before presenting them as definitive.

The dataset covers Beats Pill and competitor products, including JBL Charge 5, Bose SoundLink Flex, DOSS Extreme Boom+, Soundcore by Anker, Bang & Olufsen Beosound, W-KING, Sennheiser, Sony, and other listed portable speakers.

**Data access:** Do not upload raw review data unless you have confirmed that redistribution is permitted. If you cannot share the dataset, provide instructions describing how it can be obtained instead.

## Tools and Technologies

- Python
- pandas and NumPy
- Matplotlib and Seaborn
- TextBlob
- NLTK VADER
- WordCloud
- Google Colab
- Gemini API for AI-assisted review summarization
- Oxylabs, as described in the project notebook

## Workflow

1. Load and combine review data.
2. Inspect data types, duplicates, missing values, dates, and product identifiers.
3. Clean and transform review fields.
4. Perform exploratory data analysis and visualize rating distributions and review trends.
5. Calculate text sentiment using TextBlob and VADER.
6. Explore frequent terms in reviews with word clouds.
7. Use Gemini AI to summarize themes from selected reviews.
8. Compare products and formulate recommendations.

## Selected Findings Reported in the Notebook

- The cleaned dataframe shown in the notebook contains 1,022 records.
- The descriptive-statistics narrative reports a mean rating of approximately 4.48, a median and mode of 5, and 77.7% five-star reviews; these figures should be recalculated from the final cleaned dataframe because the notebook contains inconsistent review totals.
- The notebook's VADER output reports the following average compound sentiment scores for selected products:
  - Bose SoundLink Flex: 0.844
  - JBL Charge 5: 0.671
  - Beats Pill: 0.650
  - Soundcore by Anker: 0.625
- The AI-assisted review summary identifies sound quality and bass, portability, and design as positive themes, while noting concerns such as distortion at high volume. These are qualitative themes from the reviewed sample, not proof of all customers' views.

## Recommendations Discussed

- Investigate sound clarity and bass performance at high volume.
- Consider giving users more equalizer (EQ) control.
- Continue communicating portability, design, and sound quality.
- Use broader and more representative feedback to validate themes before making product or marketing decisions.

## How to Run

1. Open the notebook in Google Colab or Jupyter.
2. Obtain the review dataset through a permitted source and update the dataset path in the notebook.
3. Install the required Python packages if they are not already available.
4. Run the cells in order and inspect the outputs.
5. If using Gemini AI, store the API key in a secure secret or environment variable named `GEMINI_API_KEY`. Never commit credentials to GitHub.

## Limitations

- Online reviews may not represent the full customer population and may overrepresent people motivated to post reviews.
- Sentiment tools can miss sarcasm, context, and product-specific meaning.
- Competitor comparisons depend on the selected products, sample sizes, and collection period.
- The notebook contains inconsistent counts in its written statistics; validate all final figures before using them in a presentation.
- AI-generated summaries should be checked against source reviews and treated as decision support rather than ground truth.

## Repository Structure

```text
beats-by-dre-consumer-insights/
├── README.md
├── notebooks/
│   └── Beats_by_Dre_Consumer_Insights_Capstone_Project.ipynb
├── images/
│   └── charts-and-insights.png
└── requirements.txt
```

Only include `data/` if the dataset is permitted to be redistributed. Add chart images to `images/` only if they are generated from the project and do not contain private information.

## References and Data Source Notes

The original notebook lists Amazon, Oxylabs, Beats by Dre, Google Colab, Gemini, pandas, NumPy, Matplotlib, Seaborn, WordCloud, and TextBlob. Add exact dataset and library documentation links, along with collection dates and any applicable terms, before publishing.
