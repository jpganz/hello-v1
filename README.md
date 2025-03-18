# hello-v1


1st
Package it 
cd charts/
helm package .
-> this will create a package with the version...

Then

Move the .tgz file to /helm-packages and then update the config

helm repo index ./helm-packages --url https://jpganz-charts.s3.amazonaws.com/


to take all packaged Helm charts (.tgz) from my helm-packages/ folder, and create an index (registry) of them, clearly setting the URL location to my S3 bucket.