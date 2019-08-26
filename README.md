# aws-image-detect
Detect cat 

AWS commit 

sls deploy 

serverless logs -f hello

###
aws s3api put-object --bucket rekognition-cat-o-no-cat --key cat1.jpg --body cat1.jpg 


###     AWS face command ####


 .  aws rekognition detect-labels --image "S3Object={Bucket=rekognition-cat-o-no-cat,Name=yonna.jpg}" --region us-east-1
 
 
 .  aws rekognition index-faces --image "S3Object={Bucket=rekognition-cat-o-no-cat,Name=yonna.jpg}" --region us-east-1 --collection-id         friends

