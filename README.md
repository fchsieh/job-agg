# Job-agg

Job Aggregator (Job Agg) is a convenient app for searching and comparing jobs from multiple sites. It updates daily and stores data from the past 7 days. Give it a try and see how it can help you in your job search!

Demo: [http://job-agg.shion.live](http://job-agg.shion.live)

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

## Serve Web App

-   Set API URL: copy `api.json.tmp` to `api.json`
-   Build Web App: `npm run build`
-   Serve Web App: `serve -s build -l <PORT>`

## Configuration

-   Copy `config.toml.tmp` to `config.toml`
-   See `config.toml`
