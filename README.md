# Data Night 13 - Bridging Notebooks and Databases

November 18 2025 | Ad Hendrikx

## Playbook life demonstration

* this demonstration is done on a Linux laptop (Docker, venv, Jupyter Notebook etc. can be installed on MS Windows / Max OS - however this is out of scope of this demonstration)
* [github repository](https://github.com/adhendrikx/data-night-013-bridging-notebooks-and-databases)
* Docker compose file (more info about [docker](https://docs.docker.com/get-started/) and [docker compose](https://docs.docker.com/compose/gettingstarted/))
* Start: `docker compose up` (stop: `docker compose down`)
* Elaborate on PostgreSQL  and Grafana containers
* Access database with `psql`: `psql -h localhost -U postgress -d postgres`
* (psql) `\dn` for schema overview
* Create Python virtual environment: `python3 -m venv ./venv`
* Activate virtual environment: `source venv/bin/activate` (deactivate: `deactiva`te) and install jupyter notebook: `pip install jupyter`
* Run jupyter: `jupyter notebook`
* Open notebook [data-night-13-antenneregister](https://github.com/adhendrikx/data-night-013-bridging-notebooks-and-databases/blob/main/notebooks/data-night-13-antenneregister.ipynb)
* Spent some words on data set (https://antenneregister.nl/viewer/)
* Connect with containerized Grafana (http://localhost:3001/) to containerized PostgreSQL database by adding c.q. configuring a new datasource
* **NB**: use IP address of PostgreSQL container as host in Grafana's datasource config (not localhost)! 
  * `docker inspect -f '{{range.NetworkSettings.Networks}}{{.IPAddress}}{{end}}' data-night13-postgres`


* Default username / password Grafana Docker container: admin / admin
* Import dashboard [Antenneregister-1763411100909.json](https://github.com/adhendrikx/data-night-013-bridging-notebooks-and-databases/blob/main/grafana-dashboards/Antenneregister-1763411100909.json)  (set datasource)

## License
No license - feel free to use this repository as you see fit.

## Project status
Prepped for [Data Night 13 - d.d. Tuesday November 18 2025](https://www.meetup.com/nl-NL/data-nights-lochal-tilburg/events/311281574/?eventOrigin=group_upcoming_events) in november 2025.
