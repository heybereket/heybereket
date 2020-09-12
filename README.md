<p align="center">
    <a href="">
        <!-- update logo -->
        <img alt="snapsaver" src="/src/static/images/snap-orange-90.png" width ="100">
    </a>
</p>

<h3 align="center">
    SnapSaver
</h3>

<p align="center">
    Download your Snapchat memories with ease.
</p>

<p align = "center">
    <a href="http://makeapullrequest.com" target="_blank"><img alt="PR Badge" src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square"></a>
</p>

## What's SnapSaver?
SnapSaver is simple mass downloader for all of your Snapchat memories. Download from the site, have them emailed to you once the download is complete, or use the command line below.

## Setting up locally 
You'll need to have python3, pip3 and gcc installed. 

Install instructions below for Centos machines. For Ubuntu, replace `yum` with `apt-get`.
```sh
$ sudo yum update # update for latest packages
$ sudo yum install -y python3 python3-pip python3-devel gcc
```

##### Clone the repo
```
$ git clone https://github.com/addissemagn/snapsaver.git
$ cd snapsaver
```

##### Initialize a virtual environment
```
$ python3 -m venv venv
```

##### Install project modules 
```
$ source venv/bin/activate 
$ pip3 install -r requirements.txt
```

## Running the app
### Website
```
$ source venv/bin/activate
$ python3 src/main.py
```
View the site at localhost:5000 🎉

### Command line
```
$ source venv/bin/activate
$ python3 src/main.py --memories_path=<path_to_memories_history_from_Snapchat>
# Ex: python3 src/main.py --memories_path=memories_history.json
```

## Options
```
--memories_path MEMORIES_PATH
                Path to memories_history.json from Snapchat
--email EMAIL
                Optional: email to send zip file to
--help          Show help message and exit
```
