# Data Night 13 - Bridging Notebooks and Databases



## Getting started

To make it easy for you to get started with GitLab, here's a list of recommended next steps.

Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!

## Playbook life demonstration

* this demonstration is done on a Linux laptop (Docket, venv, Jupyter Notebook etc. can be installed on MS Windows / Max OS - this is out of scope of this demonstration - however if you're trying to set this up and encounter issues → contact me)
* show docker compose file (more info about [docker](https://docs.docker.com/get-started/) and [docker compose](https://docs.docker.com/compose/gettingstarted/))
* Start: `docker compose up` (stop: `docker compose down`)
* Elaborate on PostgreSQL  and Grafana containers
* access database with `psql`: `psql -h localhost -U postgress -d postgres`
* (psql) `\dn` for schema overview
* Create Python virtual environment: `python3 -m venv ./venv`
* activate virtual environment: `source venv/bin/activate` (deactivate: `deactiva`te)
* install jupyter notebook: `pip install jupyter`
* run jupyter: `jupyter notebook`
* open notebook *data-night-13-antenneregister*
* spent some words on data set (https://antenneregister.nl/viewer/)
* 





* Default username / password Grafana Docker container: admin / admin

## License
No license - feel free to use this repository as you see fit.

## Project status
Once prepped for [Data Night 13 - d.d. Tuesday November 18 2025](https://www.meetup.com/nl-NL/data-nights-lochal-tilburg/events/311281574/?eventOrigin=group_upcoming_events).
