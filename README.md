# AWS High-Availability Web Hosting

## Project Overview

This project demonstrates how to host a highly available web application using AWS services. It uses an Application Load Balancer and an Auto Scaling Group to distribute incoming traffic and maintain EC2 instance availability.

## AWS Services Used

| AWS Service | Purpose |
|---|---|
| Amazon VPC | Isolated network environment |
| Subnets | Network segmentation across Availability Zones |
| Internet Gateway | Internet connectivity |
| EC2 | Hosts the web application |
| Application Load Balancer | Distributes incoming HTTP traffic |
| Target Group | Registers and monitors EC2 instances |
| Launch Template | Defines EC2 launch configuration |
| Auto Scaling Group | Maintains and replaces instances |
| CloudWatch | Monitors AWS resources |
| SNS | Sends notifications |

## Architecture

The application follows this request flow:

Internet → Application Load Balancer → Target Group → EC2 Instances

The EC2 instances run Nginx and serve the website.

The Auto Scaling Group maintains the required instance capacity, while CloudWatch monitors resource metrics and SNS is configured for notifications.

## Project Features

- Highly available web hosting architecture
- Load balancing across EC2 instances
- Automatic instance replacement
- Auto Scaling configuration
- CloudWatch monitoring and alarms
- SNS notification integration

## Project Screenshots

All AWS implementation screenshots are available in the `screenshots/` folder.

## Documentation

For detailed implementation steps, architecture, testing and configuration, see:

`docs/AWS_High_Availability_Web_Project_Full_Documentation.pdf`

## Technologies

- Amazon Web Services (AWS)
- Amazon Linux 2023
- Nginx
- Git
- GitHub

## Author

Bikram Keshari Dakua