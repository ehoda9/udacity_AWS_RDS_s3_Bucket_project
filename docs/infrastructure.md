# AWS Services [infrastructure]
### RDS 
- The application server use AWS RDS for storing and retrieving sensitive data from postgres database.

### EBS
- Server[BACKEND] is deployed on AWS Elastic Beanstalk.
- Backend URL: `http://udagram-api-dev.eba-3qys4stt.us-east-1.elasticbeanstalk.com/api/v0`

### S3 Bucket
- Server[FRONTEND] is deployed on AWS S3 Bucket for end user. 
- Frontend URL: `http://udagram-dexter.s3-website-us-east-1.amazonaws.com/home`
