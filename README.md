# Picnic planner

This is a picnic planner app for Germany. This opens an API which takes in a range of dates (from and to) in the ISO 8601 format (e.g. 2022-05-01) and 4 preferred location for picnic in human-readable string format (e.g. Mauerpark, Berlin), calls open source [weater API][https://brightsky.dev/] to extract weather conditions on the preferred dates and returns dates and locations which are optimal for a picnic!

Happy picnic planning!

# Installing on your device and running:

Make sure you have python 3 (3.8 preferred) nstalled in your device. install the package with the command:
```
pip install api2api
```
then run with:

```
make run_api2api
```
You'll get your terminal running and a message like 'Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)....'

Copy and paste the url on your browser, append with /docs (open http://127.0.0.1:8000/docs) and voila you've the interface to perform your query!



Please document the project the better you can.

# Startup the project

The initial setup.

Create virtualenv and install the project:
```bash
sudo apt-get install virtualenv python-pip python-dev
deactivate; virtualenv ~/venv ; source ~/venv/bin/activate ;\
    pip install pip -U; pip install -r requirements.txt
```

Unittest test:
```bash
make clean install test
```

Check for api2api in gitlab.com/{group}.
If your project is not set please add it:

- Create a new project on `gitlab.com/{group}/api2api`
- Then populate it:

```bash
##   e.g. if group is "{group}" and project_name is "api2api"
git remote add origin git@github.com:{group}/api2api.git
git push -u origin master
git push -u origin --tags
```

Functionnal test with a script:

```bash
cd
mkdir tmp
cd tmp
api2api-run
```

# Install

Go to `https://github.com/{group}/api2api` to see the project, manage issues,
setup you ssh public key, ...

Create a python3 virtualenv and activate it:

```bash
sudo apt-get install virtualenv python-pip python-dev
deactivate; virtualenv -ppython3 ~/venv ; source ~/venv/bin/activate
```

Clone the project and install it:

```bash
git clone git@github.com:{group}/api2api.git
cd api2api
pip install -r requirements.txt
make clean install test                # install and test
```
Functionnal test with a script:

```bash
cd
mkdir tmp
cd tmp
api2api-run
```
