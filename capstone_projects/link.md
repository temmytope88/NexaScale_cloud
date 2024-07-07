# Cloud Resume Project

The link to my cloud resume created on AWS: [text](https://d3mvbebyy1ar02.cloudfront.net)

The resources used are:

1. AWS S3 bucket for hosting the static webpage for the resume and it is not publicly accessible.
2. AWS CloudFront, it is use to access the S3 bucket.
3. AWS RDS (Mysql), this is used to store te count of the number of visitors to the site.
4. AWS Lambda, it is used to write the backend for the application that update and fetch data from the mysql database.
5. AWS API Gateway, this is used to trigger the Lambda function when the webpage is visited

![alt text](<Screenshot 2024-07-07 064816.png>)
