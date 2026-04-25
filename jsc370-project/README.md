# JSC370 Final Project: Predicting TTC Subway Delay Lengths

This project seeks to use modelling, statistical testing, and (mostly) interactive visuals to highlight the relationship between the duration of TTC subway delays and various features, such as weather information or the cause of delays. This analysis could hopefully help stakeholders (i.e. commuters and the TTC) plan accordingly in order to reduce the impact, if not also the frequency, of subway delays.

## How to View the Report

- The full version of the report is available at https://nevin-11.github.io/jsc370-project/project.html.
- The shortened, PDF version of the report is viewable at https://nevin-11.github.io/jsc370-project/project_pdf.pdf.

## Datasets:

- TTC Subway Delay dataset (via API): https://open.toronto.ca/dataset/ttc-subway-delay-data/ under the "TTC Subway Delay Data since 2025" subsection; code to pull from API is viewable at the "For Developers" sub-subsection thereof.
- Station co-ordinates datasets: Unofficially compiled in 2005 by the *We Saw a Chicken...* blog. The blog post about the datasets (one each for Lines 1 to 4) is viewable at https://scruss.com/blog/2005/12/14/toronto-subway-station-gps-locations.
    - Line 1 (Downsview/Sheppard West to Finch): http://scruss.com/wordpress/wp-content/yonge-university-spadina-NAD83.csv
    - Co-ordinates for Line 1 stations between Downsview Park to Vaughan Metropolitan Centre (inclusive) is embedded directly in the *project.qmd* and *project_pdf.qmd* files.
    - Line 2: http://scruss.com/wordpress/wp-content/bloor-danforth-NAD83.csv
    - Line 4: http://scruss.com/wordpress/wp-content/sheppard-yonge-NAD83.csv
- TTC ridership data: The original data is available in PDF format at https://cdn.ttc.ca/-/media/Project/TTC/DevProto/Documents/Home/Transparency-and-accountability/Subway-Ridership-20232024.pdf?rev=4424b4bf53e443bd85031beab56649b7. I have then converted it to a CSV file stored at data/ttc_ridership.csv.
- Meaning of TTC subway delay codes: https://open.toronto.ca/dataset/ttc-subway-delay-data/ under the "Code Descriptions" subsection; the CSV file can be directly downloaded in that subsection. The dataset is also pre-downloaded and stored at data/Code Descriptions.csv.
- OpenMeteo hourly Toronto weather dataset: https://open-meteo.com/en/docs/historical-weather-api?timezone=America%2FNew_York&latitude=43.7064&longitude=-79.3986&start_date=2025-01-01&end_date=2025-12-31&hourly=temperature_2m,precipitation,rain,snowfall,relative_humidity_2m,wind_speed_10m; the dataset can be downloaded via the "Download CSV" button on the website. The dataset is also pre-downloaded and stored at data/open-meteo-43.69N79.41W165m.csv