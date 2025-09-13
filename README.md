# CFT-EC2

A collection of AWS CloudFormation Templates (CFT) to provision and manage EC2 instances efficiently.

## Features

- Launch EC2 instances with customizable parameters (AMI, instance type, key pairs, security groups)
- Supports tagging, IAM roles, and user data scripts
- Example templates for single and multiple instance deployments
- Modular and easy to extend for advanced configurations

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Saurabhmishra-devops/CFT-EC2.git
   ```

2. **Review and Customize the Template:**
   - Edit parameters as needed in the CloudFormation YAML/JSON files.
   - Update resource specifications for your requirements.

3. **Deploy via AWS Console or CLI:**
   - **Console:** Upload the template in AWS CloudFormation and follow the wizard.
   - **CLI Example:**
     ```bash
     aws cloudformation create-stack --stack-name MyEC2Stack --template-body file://ec2-instance.yaml --parameters ParameterKey=InstanceType,ParameterValue=t2.micro
     ```

## Example Templates

- `ec2-instance.yaml`: Launches a single EC2 instance with basic configuration.
- `multi-ec2.yaml`: Provisions multiple EC2 instances in one stack.
- `ec2-with-iam.yaml`: EC2 instance with attached IAM role.
- `ec2-with-sg.yaml`: EC2 instance with custom Security Group rules.

## Parameters

| Parameter      | Description                        | Default    |
|----------------|------------------------------------|------------|
| InstanceType   | EC2 instance type                  | t2.micro   |
| KeyName        | SSH key pair name                  | -          |
| AmiId          | AMI ID for the EC2 instance        | -          |
| VpcId          | VPC to launch the instance in      | -          |

## Contributing

Contributions are welcome! Fork the repo, create a branch, and submit a pull request.

## License

This project is licensed under the MIT License.

## Author
Saurabh Mishra

[Saurabhmishra-devops](https://github.com/Saurabhmishra-devops)
