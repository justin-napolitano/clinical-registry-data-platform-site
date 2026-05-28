# Local Registry Platform Showcase

Local interview walkthrough site for the clinical registry data platform.

## Run

From the `registry-mapping-review-console` repo:

```bash
python -m http.server 8080 --directory showcase/local-registry-website
```

Open:

```text
http://localhost:8080
```

## Optional STS Streamlit App

In a second terminal:

```bash
uv run streamlit run tools/mapping_review_app.py --server.port 8501
```

Then use the showcase launchpad to open:

```text
http://localhost:8501
```
