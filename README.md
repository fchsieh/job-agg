# Job-agg

Aggregator for job searching

## Usage

-   Clone this repo with submodules

```
git clone --recurse-submodules
```

## Dependencies

-   Install python packages

```
cd linkedin-scraper && pip install -r requirements.txt
```

-   Set up MongoDB
-   Download the Firebase credential file and rename it into `firebase.json`, and put it under this directory

## Scrap LinkedIn jobs

```
cd linkedin-scraper && python ./main.py
```

## Start Backend API server

```
cd job-agg-backend && go run main.go
```

## Configuration

-   Copy `config.toml.tmp` to `config.toml`
-   See `config.toml`
