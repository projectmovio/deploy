# Pre requirements

* Make sure you are authorized to AWS. See: http://docs.aws.amazon.com/cli/latest/userguide/cli-config-files.html


# Deploy steps

* docker build -t movio:1.0 .
* docker run -i -t movio:1.0 create cluster --zones eu-west-1a movio.k8s.local
* docker run -i -t movio:1.0 update cluster movio.k8s.local --yes