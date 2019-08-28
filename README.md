# aws-image-detect
Detect cat 

AWS commit 

sls deploy 

serverless logs -f hello

###
aws s3api put-object --bucket rekognition-cat-o-no-cat --key cat1.jpg --body cat1.jpg 


###     AWS face command ####

#######Detect image label
 .  aws rekognition detect-labels --image "S3Object={Bucket=rekognition-cat-o-no-cat,Name=yonna.jpg}" --region us-east-1
 
 
######Detect face lable change to collection  
 .  aws rekognition index-faces --image "S3Object={Bucket=rekognition-cat-o-no-cat,Name=yonna.jpg}" --region us-east-1 --collection-id         friends
 
#####Find face by s3 bucket image  
 .  aws rekognition search-faces-by-image --collection-id friends --image "S3Object={Bucket=rekognition-cat-o-no-cat,Name=yonna.jpg}"

######Search Face list
.   aws rekognition list-faces --collection-id friends

######Search Face by id 
.  aws rekognition search-faces --collection-id friends --face-id abe1915e-aa20-43c6-8491-7ddc17ff5efe
