# EatSure Complaint Intelligence

Multilingual and code-mixed complaint analysis using character-level TF-IDF and classical machine learning. The app includes single and batch analysis, optional English translation, confidence-based review guidance, and interactive complaint insights.

## Run locally

```bash
pip install -r requirements.txt
streamlit run app.py
```

The app requires the model bundle and the three dashboard aggregate CSV files beside `app.py`. Translation is optional and requires internet access.

## Dashboard data and privacy

The public dashboard exports only grouped counts: month/category/language, category/subcategory, and overall priority/sentiment/resolution/channel totals. Every published aggregate group has at least five records. It contains no raw complaint text, customer or order identifiers, city, or brand fields. Uploaded batch files are processed in the app session and can be downloaded by the user; they are not included in this repository.

## Deploy

In Streamlit Community Cloud, select this repository and set the app entry point to `app.py`.
