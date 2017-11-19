# Pre requirements

* Make sure you are authorized to AWS. See: http://docs.aws.amazon.com/cli/latest/userguide/cli-config-files.html
* docker build -t movio:1.0 .

# Running locally
* Pull down all projectmovio repositories one folder up relative this one.
* `docker-compose up` 

# Deploy steps

* docker run -i -t movio:1.0 create cluster --zones eu-west-1a movio.k8s.local
* docker run -i -t movio:1.0 update cluster movio.k8s.local --yes

# Teardown steps

* docker run -i -t movio:1.0 delete cluster --name movio.k8s.local --yes