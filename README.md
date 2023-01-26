# Job-agg

Job Aggregator (Job Agg) is a convenient app for searching and comparing jobs from multiple sites. It updates daily and stores data from the past 7 days. Give it a try and see how it can help you in your job search!

Demo: [https://job-agg.shion.live](https://job-agg.shion.live)

## Features

-   Run a job search on multiple sites at once, and save the results to your Firebase
-   Cache the results in your MongoDB for better performance
-   Display the results in a web app with a clean and simple UI

## Usage

### 1. Scrap Job Data

```
cd job-agg-scraper && python3 ./main.py
```

### 2. Start Backend API server

```
cd job-agg-backend && go run main.go
```

### 3. Serve Web App

-   Set API URL: copy `api.json.tmp` to `api.json`
-   Serve Web App: `cd job-agg-frontend && npm run start`

## Configuration

-   Copy `config.toml.tmp` to `config.toml`, and `firebase.json.tmp` to `firebase.json`
-   See `config.toml` for more details

## Docker

Alternatively, you can use docker-compose to run the web app and backend API server.

First, configure the `config.toml` and `firebase.json` files as described above, and change the settings in `docker-compose.yml` if necessary.

Then, copy `config.toml.tmp` to `job-agg-backend/config.toml`, and `firebase.json.tmp` to `job-agg-backend/firebase.json`.

Finally, run the following command to start the containers:

```
docker-compose up
```

After the containers are up, you can access the web app at [http://localhost:3000](http://localhost:3000).

## License

[MIT](https://choosealicense.com/licenses/mit/)
