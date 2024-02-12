# AWS Lambda Data Processing Function in Rust

## Overview

This AWS Lambda function is written in Rust and is designed to process and transform sample data. It uses `Cargo Lambda` for easy deployment and management of the Lambda function. The function is integrated with API Gateway to enable HTTP requests handling.

## Requirements

- Rust Lambda Function using `Cargo Lambda`.
- Ability to process and transform sample data.

## Getting Started

To get started with this project, you'll need to have Rust installed, as well as the `cargo-lambda` extension for Rust. This will facilitate building, deploying, and managing your AWS Lambda functions.

## Deployment

1. **Install Cargo Lambda:**
  
  If you have not already installed `cargo-lambda`, you can do so with the following command:
  
  ```bash
  cargo install cargo-lambda
  ```
  
2. **Build the Function:**
  
  Build the Lambda function using Cargo with the `cargo-lambda` extension.
  
  ```bash
  cargo lambda build --release
  ```
  
3. **Deploy to AWS Lambda:**
  
  After building, use `cargo-lambda` to deploy the function to AWS Lambda.
  
  ```bash
  cargo lambda deploy
  ```
  

## API Gateway Integration

This Lambda function is integrated with API Gateway, making it accessible via HTTP. The function processes query string parameters to generate responses based on input data.

## Example Invocation

After deployment, send a request with a query parameter to process the data:

```bash
curl "https://tt5a6xsco2uzt32vzmb6jdijie0mbuxj.lambda-url.us-east-1.on.aws?name=SampleName"
```

## Documentation

The README.md documentation provides all the necessary information to understand how the function processes data and how it's integrated with API Gateway. It also includes instructions on how to deploy and invoke the function.
