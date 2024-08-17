# Metrics With Prometheus

TODO: Intro

## Setup

* Install `gum` by following the instructions in https://github.com/charmbracelet/gum#installation.

```bash
chmod +x metrics/prometheus.sh

./metrics/prometheus.sh
```

## Do

```sh
echo "http://prometheus.$INGRESS_HOST"
```

* Open it in a browser

```sh
echo "http://grafana.$INGRESS_HOST"
```

* Open it in a browser
* Use `admin` as the user and `prom-operator` as the password
* Explore dashboards

```sh
curl "http://simple-app.$INGRESS_HOST"

curl "http://simple-app.$INGRESS_HOST/videos"

curl -X POST "http://simple-app.$INGRESS_HOST/video?id=-qeoLfSGlFU&title=DevOps%20Tools%202024"

curl "http://simple-app.$INGRESS_HOST/videos" | jq .

echo "http://simple-app.$INGRESS_HOST"
```

* Use that URL to generate some load using https://ddosify.com or any other load-testing tool
* See the results in Grafana dashboards

## Continue the Adventure
