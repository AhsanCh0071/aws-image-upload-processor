# aws-image-upload-processor

# 🖼️ AWS Serverless Image Upload & Processing App

This is a simple serverless application that allows users to upload images to an S3 bucket. Once uploaded, an AWS Lambda function automatically processes (resizes/compresses) the image and stores it in a `/resized` folder within the same bucket.

---

## 🔧 Technologies & AWS Services Used

- **Amazon S3** – for storing original and processed images  
- **AWS Lambda** – for automatic image processing  
- **IAM Roles** – for secure access between services  
- **CloudWatch Logs** – to monitor Lambda events  

---

## 📂 Project Structure

aws-image-upload-processor/
├── index.html # Upload form
├── lambda_function/ # Contains image processing code
│ └── lambda-function.py # Lambda function script
├── README.md # Project details and setup


---

## 🚀 How It Works

1. User uploads an image via the HTML form.  
2. The image is stored in the `original/` folder in S3.  
3. S3 triggers the Lambda function.  
4. Lambda resizes/compresses the image.  
5. Processed image is saved in `processed/` folder.  

---

## 🧪 How to Test

- Open `index.html` in your browser.  
- Upload an image.  
- Go to your S3 bucket → check `original/` and `processed/` folders.  

---

## 📊 Cost

- This app is designed to stay within the **AWS Free Tier** limits.  
- No charge if used lightly during testing.  

---

## ✅ Status

✅ Project Completed  
🔜 Improvements: Add API Gateway & authentication  

---

## 🙌 Author

**Ahsan Ullah** – [GitHub](https://github.com/AhsanCh0071)
