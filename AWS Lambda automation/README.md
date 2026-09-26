# 🚀 Automated Data Export Pipeline

An automated AWS data export pipeline designed to retrieve data
from Amazon RDS, generate a CSV file, store it in Amazon S3,
and send the exported data through Amazon SES.

## 🏗️ Architecture

The solution follows an event-driven architecture.

```text
Amazon EventBridge
        ↓
    AWS Lambda
        ↓
   Amazon RDS
        ↓
    Generate CSV
        ↓
    Amazon S3
        ↓
    Amazon SES
