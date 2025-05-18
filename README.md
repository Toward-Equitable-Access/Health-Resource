# [Toward Equitable Access: Leveraging Crowdsourced Reviews to Investigate Public Perceptions of Health Resource Accessibility](https://arxiv.org/pdf/2502.10641)

Access to health resources is a critical determinant of public well-being and societal resilience, particularly during public health crises when demand for medical services and preventive care surges. However, disparities in accessibility persist across demographic and geographic groups, raising concerns about equity. Traditional survey methods often fall short due to limitations in coverage, cost, and timeliness. This study leverages crowdsourced data from Google Maps reviews, applying advanced natural language processing techniques, specifically DeBERTa, to extract insights on public perceptions of health resource accessibility in the United States during the COVID-19 pandemic. Additionally, we employ Partial Least Squares regression to examine the relationship between accessibility perceptions and key socioeconomic and demographic factors—including political affiliation, racial composition, educational attainment and so on. Our findings reveal that public perceptions of health resource accessibility varied significantly across the U.S., with disparities peaking during the pandemic and slightly easing post-crisis. Political affiliation, racial demographics, and education levels emerged as key factors shaping these perceptions. These findings underscore the need for targeted interventions and policy measures to address inequities, fostering a more inclusive healthcare infrastructure that can better withstand future public health challenges.

## Notebook Descriptions:

### `1.data-processing.ipynb`
*   **Purpose**: Collects and cleans Google Maps review data for stores across 49 U.S. states.

### `2.text-classification.ipynb`
*   **Purpose**: Trains and evaluates various text classification models to categorize the sentiment of the filtered health resource-related reviews.

### `3.county-result.ipynb`
*   **Purpose**: Aggregates the classified review sentiments to the U.S. county level and prepares data for spatio-temporal analysis.

### `4.pls-regression.ipynb`
*   **Purpose**: Investigates the relationship between county-level sentiment scores (for pre-COVID, during-COVID, and post-COVID periods) and various socio-economic factors using Partial Least Squares (PLS) Regression.

### `5.result-validation.ipynb`
*   **Purpose**: Prepares data for validating the Google Maps review-based sentiment scores against external survey data, by aggregating review sentiments at the state-month level.

### `6.survey-validation.ipynb`
*   **Purpose**: Validates the Google Maps review-based sentiment by comparing it with external survey data on delayed medical care.

### `7.plot-gis-moran.ipynb`
*   **Purpose**: Visualizes the geographic distribution of county-level sentiment scores using GIS maps and analyzes spatial autocorrelation using Moran's I.
