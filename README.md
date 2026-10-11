# cae.duckdb
Shared DuckDB Instance for the City Analytics Exchange Community

<img width="577" height="160" alt="image" src="https://github.com/user-attachments/assets/c3c0d7d4-182a-4963-9697-8179e2b90c06" />  

## Try it Out
You can quickly start querying the data by clicking [here](https://shell.duckdb.org/#queries=v0,ATTACH-'https%3A%2F%2Fraw.githubusercontent.com%2FDanielJDufour%2Fcae.duckdb%2Frefs%2Fheads%2Fmain%2Fcae.duckdb'-AS-cae~,SELECT-name%2Clatitude%2Clongitude-FROM-cae.bike_chattanooga_stations_v1-LIMIT-5~)

## Contributing
You can add a dataset in these 3 simple steps:
1. convert it to [parquet](https://parquet.apache.org/)
2. Upload the parquet file to Github, AWS S3, or some place where it gets a static URL with CORS enabled.
3. Submit a PR to [datasets.csv](https://github.com/DanielJDufour/cae.duckdb/blob/main/datasets.csv)

## Import
You can add this database into your own DuckDB instance with one line by using DuckDB's attach mechanism:
```
ATTACH 'https://raw.githubusercontent.com/DanielJDufour/cae.duckdb/refs/heads/main/cae.duckdb' AS cae;
```

## Download
You can directly download the database here:  
https://github.com/DanielJDufour/cae.duckdb/blob/main/cae.duckdb
