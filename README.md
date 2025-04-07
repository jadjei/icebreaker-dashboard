
Configure prometheus to pull metrics from your Icebreaker server and port.

/etc/prometheus/prometheus.yml
```
  - job_name: 'icebreaker'
    scrape_interval: 5s
    static_configs:
      - targets: ['mainnet-relay2:3030']
```

In Grafana, on the Dashboards page, click New -> Import and paste the contents of icebreaker.json into the "Import via dashboard JSON model" field.
