# docker sabnzbd
This is a Dockerfile to set up "SABnzbd" - (http://sabnzbd.org/)
Build from docker file
```
git clone https://github.com/jongillies/docker-sabnzbd.git
cd docker-sabnzbd
docker build -t sabnzbd .
```

docker run -d \
    -v $SABNZDB_CONFIG:/config \
    -v $SABNZDB_DATA:/data \
    -v $SABNZDB_INCOMPLETE:/incomplete \
    -v $SABNZDB_COMPLETE:/complete \
    -p 8080:8080 -p 9090:9090 --name sabnzbd sabnzbd

Fire up the web ui.

Setup your Usenet server.
Setup the login creds
...
Restart

Navigate to config/folders

set /incomplete
/complete
...
