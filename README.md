# ChurnBuster

ChurnBuster is an automated data processing project designed to streamline the extraction, transformation, and loading (ETL) of customer churn data using Apache Airflow and AWS Glue. This project helps organizations proactively analyze and address customer churn by automating the data processing pipeline, making it easier to gain insights into customer behavior and take action to reduce churn rates.

## Project Features

- **Automation:** ChurnBuster automates the entire ETL process, reducing manual effort and ensuring consistent, reliable data processing.

- **Customizable Scheduling:** The project offers customizable scheduling options, allowing organizations to choose how frequently they want to analyze customer churn data.

- **Real-time Monitoring:** ChurnBuster provides real-time monitoring of AWS Glue job execution, giving users immediate visibility into job status and outcomes.

- **Scalability:** Built on AWS Glue and Apache Airflow, the project is highly scalable, making it suitable for organizations of all sizes.

## Prerequisites

Before getting started with ChurnBuster, make sure you have the following prerequisites in place:

- Python 3.x
- Apache Airflow
- Boto3 (Python SDK for AWS)
- AWS Glue
- AWS IAM credentials (access key and secret key)

## Configuration

### DAG Configuration

- `owner`: The owner of this DAG (change to your name).
- `start_date`: The start date for the DAG (set to your desired start date).
- `retries`: Number of retries upon failure.
- `retry_delay`: Delay between retries.

### AWS Glue Configuration

- Replace the placeholder values in the `boto3.client` call with your own AWS IAM credentials and region.
- Ensure that your AWS IAM user has the necessary permissions to start and monitor Glue jobs.

## Usage

Follow these steps to set up and use ChurnBuster:

1. Clone the ChurnBuster project repository to your local environment.

2. Configure your AWS credentials and Glue job parameters in the project's configuration files.

3. Set up an Apache Airflow environment and ensure you have the necessary dependencies installed.

4. Create a DAG run in Airflow, specifying the job name for the ETL process.

5. Monitor the DAG execution logs to track the progress of the ETL job.

6. Use the insights generated by ChurnBuster to make informed decisions and reduce customer churn rates.

## Security Disclaimer

It's essential to follow best practices for managing AWS credentials and ensure the security of sensitive data during the ETL process. Avoid hardcoding credentials in your project and consider using Airflow's built-in support for secrets management.

## Project Author

- Author: [Your Name]

## License

This project is licensed under the [License Name] - see the [LICENSE.md](LICENSE.md) file for details.
