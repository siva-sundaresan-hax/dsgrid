# Docker Selenium Grid

CLI program for building and managing a Selenium Grid with Docker containers.

## Requirements

* Docker
* Python 2.7

## Installation

```bash
git clone https://github.com/brady-vitrano/dsgrid.git
cd dsgrid
python setup.py install
dsgrid install
```

## Usage

```
# Start the Hub
dsgrid start
# Add Nodes
dsgrid nodes add firefox
dsgrid nodes add phantomjs
# Restart Nodes by Browser
dsgrid nodes restart firefox
# Restart All Nodes
dsgrid nodes restart
# Check Status
dsgrid status
# Shutdown
dsgrid shutdown
```

View the Grid console on: http://localhost:49044/grid/console


## Author Note

I put this together over a weekend. I am not very strong in Python but wanted to build a CLI app which can be easily
installed on Docker hosts.

The tests are incomplete. What you see are my TDD leftovers.

## Missing/TODO

* Fix tests
* Add logging and debugging options
* Add ChromeDriver
* Add CLI usage help with tabcomplete
* Add documentation on configuring Dockerfiles for custom Selenium settings ie proxy, timeouts, etc

