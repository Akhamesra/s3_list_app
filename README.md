# s3_list_app
## A Flask app to list the contents of a S3 bucket.
1. GET /list-bucket-content/: Returns the top-level content of the S3 bucket.
2. GET /list-bucket-content/<path>: Returns the contents of a specific path.
3. If the path does not exist, it returns a Non-existing path message.

## Assumption 
1. Code will use the Role of the server to get the permission of S3 bucket.
#### OR
2. Code will use the already configured aws credentials (default) in (~/.aws/credentials).

## Requirements
1. Boto3
2. Flask

## Steps to run application 
```
git clone https://github.com/Akhamesra/s3_list.git
cd s3_list
pip3 install -r requirements.txt
nohup python3 app.py &
```

#### Application will run on port 5000
