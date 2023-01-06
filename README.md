# Job-agg

Aggregator for job searching

## Dependencies

-   Install python packages

```
cd linkedin-scraper && pip install -r requirements.txt
```

-   Set up MongoDB
-   Download Firebase credential and rename into `firebase.json`

## Scrap LinkedIn jobs

```
cd linkedin-scraper && python ./main.py
```

## Start Backend API server

```
cd job-agg-backend && go run main.go
```

## Configuration

See `config.toml`
