oracle-py3-gcloud-pandas
========================
A debian:jessie slim container with cx_oracle client, python3, pandas, gcloud big query dependencies


to add your own dependencies
----------------------------
1. Clone the repository
1. edit `requirements.txt`
1. `docker build -t oracle-py3-gcloud-pandas docker/.`


to use the image (assuming your current directory contains the python scripts you want to run)
----------------------------------------------------------------------------------------------
```
docker run --rm -e GOOGLE_APPLICATION_CREDENTIALS=/home/key.json -v "`pwd`":"/home" oracle-py3-gcloud-pandas python3 /home/myScript.py
```


Licensing
-------------
[Oracle Instant Client license](hhttp://www.oracle.com/technetwork/licenses/distribution-license-152002.html)

Note
----
Inspired from  [hjaf23 image](https://github.com/hjaf23/docker-cx_Oracle)
