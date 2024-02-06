# ML Flow Simple Tutorial


## TODO:

- Add MLflow to S3:
    1. Login to AWS console.
    2. Create IAM user for deployment
    3. Create ECR repo to store/save docker image
    4. Create EC2 machine (Ubuntu)
    5. Create, into inbound security group, port 5000 (TCP)
    5. Create s3 bucket to store artifacts
    6. Open EC2 and Install docker in EC2 Machine
    7. Run the following command in EC2:
        sudo apt update
        sudo apt install python3-pip
        sudo pip3 install pipenv
        sudo pip3 install virtualenv
        mkdir mlflow
        cd mlflow
        pipenv install mlflow
        pipenv install awscli
        pipenv install boto3
        pipenv shell

        ## Then set aws credentials
        aws configure

        #Finally
        mlflow server -h 0.0.0.0 --default-artifact-root **your s3 bucket name**

        #set uri in your local terminal and in your code
        export MLFLOW_TRACKING_URI= **your mlflow tracking uri**
    7. Configure EC2 as self-hosted runner
    8. Setup github secrets











