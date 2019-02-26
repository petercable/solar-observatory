# solar-observatory
Monitoring system for Enphase envoy-based photovoltaic systems

## Setup instructions

* install docker and docker-compose
* set ENVOY_HOST (ip address for your envoy) and ENVOY_PASS
* in prometheus/prometheus.yml set the `targets` for the `node-exporter` job (if you want to monitor your host machine)
* `docker-compose build scraper`
* `docker-compose up -d`


I have 3 rows of panels, so I have some location labeling for these 3 arrays. If you wish to label your panels
just replace the `serials` map in scrape.py and rebuild the container.
