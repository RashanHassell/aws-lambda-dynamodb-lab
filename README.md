# aws-lambda-dynamodb-lab
AWS Lambda function triggered by S3 uploads, writing metadata to DynamoDB
# AWS Lambda to DynamoDB Integration

This project demonstrates a serverless workflow using AWS services. When a file is uploaded to an S3 bucket, an AWS Lambda function is triggered to log the file's metadata into a DynamoDB table.

## 🛠️ Technologies Used

- **Amazon S3**: Triggers the Lambda function upon file upload.
- **AWS Lambda**: Processes the S3 event and extracts file metadata.
- **Amazon DynamoDB**: Stores the file metadata (`filename`, `filesize`, `upload_time`).
- **Amazon CloudWatch**: Logs Lambda function execution details.

## 📂 Project Structure

- `lambda_function.py`: Contains the Lambda function code.
- `README.md`: Project documentation.
- `screenshots/`: Directory containing screenshots of the implementation.

## 🔄 Workflow

1. A file is uploaded to the designated S3 bucket.
2. The S3 event triggers the Lambda function.
3. The Lambda function extracts the file's metadata.
4. The metadata is stored as an item in the DynamoDB table.

## 📸 Screenshots

### Lambda Function Code

![Screenshot 2025-05-02 132233](https://github.com/user-attachments/assets/454acda3-99e7-4715-8031-9cabededf5bf)


### CloudWatch Log Output

![Screenshot 2025-05-02 132120](https://github.com/user-attachments/assets/98f992aa-66ee-4c40-9b32-efa328c2fe04)


### DynamoDB Table Entry

![Screenshot 2025-05-02 132011](https://github.com/user-attachments/assets/21ee7509-6ea6-4518-ae0b-84c6c9e55341)


## ✅ Skills Demonstrated

- Serverless architecture implementation.
- Event-driven programming with AWS services.
- Integration of AWS Lambda with DynamoDB using Boto3.
- Monitoring and logging with Amazon CloudWatch.
