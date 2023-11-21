# Class 37

## Introduction to Amazon S3

1. What is Amazon S3?

Amazon Simple Storage Service (Amazon S3) is an object storage service provided by AWS, offering scalable, secure, and highly durable storage. It allows customers to store and retrieve any amount of data, such as images, videos, and documents, through a web interface or various AWS SDKs.

2. List at least 3 features that it offers to its users.

Storage Classes: Amazon S3 provides different storage classes tailored for various use cases, allowing users to optimize costs based on data access patterns. Examples include S3 Standard, S3 Standard-IA, S3 One Zone-IA, S3 Glacier, etc.
Access Management and Security: Users can control access to their buckets and objects using features like AWS Identity and Access Management (IAM), bucket policies, access points, and more. Security features like S3 Block Public Access and Object Lock enhance data protection.
Data Processing: Amazon S3 supports features like S3 Object Lambda, allowing users to add custom code to modify and process data during GET, HEAD, and LIST requests. Event notifications enable triggering workflows using services like Amazon SNS, Amazon SQS, and AWS Lambda.

3. What is an object key?

An object key is the unique identifier for an object within an Amazon S3 bucket. It is essentially the name of the object and, along with the bucket name, forms a unique address for each stored object. The combination of bucket name, object key, and optionally, a version ID (if versioning is enabled) uniquely identifies each object in Amazon S3. For example, in the URL `https://DOC-EXAMPLE-BUCKET.s3.us-west-2.amazonaws.com/photos/cat.jpg`, "`photos/cat.jpg`" is the object key.

---

## S3 with Amplify

1. Which dependencies are needed to install Amplify AWS S3 to your ndroid application?

- `com.amplifyframework:aws-storage-s3:2.14.5`
- `com.amplifyframework:aws-auth-cognito:2.14.5`

2.What is needed in order to upload data to your bucket?

- The key is specified as "ExampleKey."
- The data object is a file named "ExampleKey" with the contents "Example file contents."

3.what method(s) initialize(s) the Amplify Auth and Storage categories?

The method that initializes the Amplify Auth and Storage categories is the `Amplify.configure()` method. In the provided code example, this method is called in the `onCreate()` method of the application class:

`Amplify.configure(getApplicationContext());`

---

## Things I want to know more about

- Advanced Amazon S3 Features
- Amplify Storage Configuration