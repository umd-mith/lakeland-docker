This repository contains a Docker setup for starting the Lakeland Omeka. 

First you'll need to get the archived Lakeland data from Amazon S3:

    aws s3 sync s3://mith-bags/A36E23C8-45E3-4ECD-8D8E-610CEDF60441/data data 

Extract the data:

    tar xvfz data/lakeland.tar.gz -C data

Get the database configuration we will use:

    cp config/db.ini data/lakeland/db.ini

Start the app (MySQL and Apache):

    docker-compose up

Go to:

    http://localhost:8000





