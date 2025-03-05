# User Data Collection and Email Sender

This Python script collects user information, validates it using regular expressions, and sends the collected details to the provided email using Gmail's SMTP server.

## Features

The script collects and validates the following details:
- **Name**: Only letters and spaces allowed
- **Date of Birth**: Format `DD-MM-YYYY`
- **Mobile Number**: 10-digit number starting with 6-9
- **Instagram ID**: No specific validation
- **Email**: Only Gmail addresses are accepted

It then sends an email with the collected details.

## Prerequisites

- Python 3.x installed
- `smtplib` and `email` modules (included in standard Python library)
- A valid Gmail account for sending emails
- Environment variables set for Gmail credentials:

  ```sh
  export SENDER_EMAIL="your-email@gmail.com"
  export SENDER_PASSWORD="your-app-password"
  ```

## Expected Input Format

| Field           | Format Example         | Validation |
|---------------|---------------------|------------|
| Name          | John Doe            | Only letters and spaces |
| Date of Birth | 25-12-1995          | DD-MM-YYYY format |
| Mobile Number | 9876543210          | 10 digits, starts with 6-9 |
| Instagram ID  | john_doe123         | Any text input |
| Email         | example@gmail.com   | Only Gmail addresses |



## Troubleshooting

If emails are not sent, ensure:
- Gmail SMTP settings allow sending emails.
- The provided credentials are correct.
- Environment variables are properly set.
- Python version is compatible.

