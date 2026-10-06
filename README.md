#AWS Serverless Web Visitor Counter

The web application is a full-stack implementation that makes use of Amazon Web Services cloud solutions to host a website that can count page visits in real time.

#Live demo:

The link to the deployed solution is http://my-visitor-app-bucket-123.s3-website.ap-south-1.amazonaws.com (S3 static website hosting).

#Architecture overview:

The application uses the following components:

1. The frontend is a simple HTML5/JS static website hosted in Amazon S3.
2. The API layer is exposed through an Amazon API Gateway that handles HTTP methods and CORS preflight requests.
3. AWS Lambda Python 3.12 runtime executes the business logic.
4. Amazon DynamoDB database is used to store the counter value with an update function that uses the PUT method to implement a server-side increment operation.
5. The custom IAM roles policy allows least-privilege access between Lambda and DynamoDB resources.

#Technologies:

The application is built using the following technologies:
- Cloud provider: Amazon Web Services (AWS)

- Programming langauges: Python, JavaScript, HTML5, CSS3

- Supporting tools: S3, API Gateway, Lambda, DynamoDB, IAM resource policy editor
