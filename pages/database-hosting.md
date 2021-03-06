# Database hosting

<!-- TOC depthFrom:2 -->

- [AWS DynamoDB](#aws-dynamodb)
- [Cloudant CouchDB](#cloudant-couchdb)
- [Firebase database](#firebase-database)
- [GearHost Database](#gearhost-database)
- [Google Cloud Datastore](#google-cloud-datastore)
- [Heroku Postgres](#heroku-postgres)
- [Heroku Redis](#heroku-redis)
- [mLab](#mlab)
- [OpenShift MongoDB](#openshift-mongodb)
- [Redis Cloud](#redis-cloud)

<!-- /TOC -->

## AWS DynamoDB

[Pricing page](https://aws.amazon.com/dynamodb/pricing/)

- *Free tier*: 25 GB of Storage, 25 Units of Write Capacity, 25 Units of Read Capacity
- *Pros*: A NoSQL database with both document and key-value store models, replicated with high availability.  The free tier is enough to handle up to 200M requests per month.
- *Limitations*: One unit of read/write capacity handles one request per second (or two requests per second in the case of eventually consistent reads). Has both strongly consistent and eventually consistent reads.

## Cloudant CouchDB

[Pricing page](https://cloudant.com/product/pricing/)

* *Free tier*: 1$/GB per month, $0.015$/100 "heavy" requests, $0.015/500 "light" requests,  first $50 per month free
* *Pros*: Full CouchDB hosting. Can host also static sites and javascript applications
* *Limitations*: Account on shared multitenant instance
* *Exceeding the free tier*: Credit card needed after first 30 days to charge exceeding usage

## Firebase database

[Pricing page](https://firebase.google.com/pricing/)

* *Free tier*: 1GB storage, 10GB/month transfer, 100 simultaneous connections
* *Pros*: really fast can be used for real time pub/sub, libraries for multiple platforms, designed to be used directly from frontend (with security rules), integrates with Firebase Authentication
* *Limitations*: no backups, limited queries, complicated security rules (read the manual!)

## GearHost Database

[Pricing page](https://www.gearhost.com/pricing)

* *Free tier*: 5MB MySQL database or 10MB MS SQL database
* *Pros*: Recent versions (MySQL 5.6, MS SQL Server 2014)
* *Limitations*: simultaneous connections seems to be limited (according to [this page](http://talk.gearhost.com/t/restrictions-or-limitations-of-the-free-account/105), approx. 15)
* *Exceeding the free tier*: The database becomes locked and a kind email is sent asking to upgrade to paid plan

## Google Cloud Datastore

[Product page](https://cloud.google.com/datastore/)

* *Free tier*: 1GB storage/day, 50K reads/day, 20K writes/day, 20K deletes/day
* *Pros*: dashboard, clients available in multiple languages, fully managed (sharding and replication), ACID transactions
* *Limitations*: complex requests needs specific indexes (read the manual)

## Heroku Postgres

[Product page](https://www.heroku.com/postgres)

* *Free tier*: 10K rows/month, 20 simultaneous connections
* *Pros*: dashboard, secured
* *Limitations*: SLA with maximum of 4 hours of downtime/month (99.5% uptime), no in-memory cache, no expensive queries support

## Heroku Redis

[Product page](https://www.heroku.com/redis)

* *Free tier*: 25MB ram, 20 connections
* *Pros*: dashboard, secured, analytics, access via Heroku CLI
* *Limitations*: SLA with maximum of 4 hours of downtime/month

## mLab

[Pricing page](https://mlab.com/plans/pricing/)

* *Free tier*: 500MB storage, daily backup
* *Pros*: managed on AWS, Azure or Google Cloud, data browser, monitoring

## OpenShift MongoDB

[Product Page](https://developers.openshift.com/databases/mongodb.html)

* *Free tier*: 1Gb storage
* *Pros*: Easy to deploy
* *Limitations*: Only support mongodb 2.4

## Redis Cloud

[Pricing page](https://redislabs.com/pricing)

* *Free tier*: 30MB, 30 connections
* *Pros*: managed, possibility to choose cloud provider (AWS, Azure, GCE, IBM Softlayer) and availability zones
