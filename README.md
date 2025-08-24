#S3 to SNS Notification Setup

Overview
This setup sends S3 bucket event notifications to an SNS topic for further processing or alerting.

Resources
S3 Bucket: img-stg121
SNS Topic: arn:aws:sns:us-east-2:256207368585:S3-event-notification

Flow
An event (e.g., object created) occurs in the S3 bucket.
The bucket publishes the event to the SNS topic.
All subscribers to the SNS topic receive the notification.

Policy
The SNS topic policy allows the S3 bucket to publish events s
