# AWS CDK Python Project
This is a sample project that demonstrates the usage of AWS CDK (Cloud Development Kit) with Python. It creates an AWS CloudFormation stack containing an Amazon SQS queue, an S3 bucket, and an SNS topic with an SQS subscription.

1. Prerequisites
Before you can deploy this project, make sure you have the following prerequisites installed and configured:

- Python 3.x
- AWS CLI (Command Line Interface)
- AWS CDK (npm install -g aws-cdk)
2. Getting Started
To get started with this project, follow these steps:

- Clone the repository to your local machine.
- Navigate to the project directory.
" cd aws-cdk-python-project "
- Install the required Python dependencies.
" pip install -r requirements.txt "
- Deploy the AWS CDK stack.
" cdk deploy "
- This command will deploy the infrastructure defined in the CdkStack class to your AWS account.

- Review the changes that will be made during the deployment. Confirm the changes if they align with your expectations and security requirements.

- Once the deployment is complete, you can verify the created resources in the AWS Management Console or by using AWS CLI commands.

# Project Structure
The project structure is as follows:

- cdk_stack.py: This file contains the main AWS CDK stack definition, including the creation of an SQS queue, an S3 bucket, and an SNS topic with an SQS subscription.
- requirements.txt: This file lists the Python dependencies required for the project.
- cdk.json: This JSON file specifies the CDK app entry point.
# Customization
Feel free to customize this project according to your requirements. You can modify the AWS resources created, add additional resources, or update the stack configuration as needed. Refer to the AWS CDK documentation for more information on how to customize CDK stacks and resources.

# Clean Up
To clean up and remove the deployed resources from your AWS account, use the following command:
" cdk destroy "
- This will delete the CloudFormation stack and all associated resources.

# License
This project is licensed under the MIT License. See the LICENSE file for details.

Feel free to update the README with additional information or instructions specific to your project.

---------------------
(generated on deploy)

# Welcome to your CDK Python project!

You should explore the contents of this project. It demonstrates a CDK app with an instance of a stack (`cdk_stack`)
which contains an Amazon SQS queue that is subscribed to an Amazon SNS topic.

The `cdk.json` file tells the CDK Toolkit how to execute your app.

This project is set up like a standard Python project.  The initialization process also creates
a virtualenv within this project, stored under the .venv directory.  To create the virtualenv
it assumes that there is a `python3` executable in your path with access to the `venv` package.
If for any reason the automatic creation of the virtualenv fails, you can create the virtualenv
manually once the init process completes.

To manually create a virtualenv on MacOS and Linux:

```
$ python -m venv .venv
```

After the init process completes and the virtualenv is created, you can use the following
step to activate your virtualenv.

```
$ source .venv/bin/activate
```

If you are a Windows platform, you would activate the virtualenv like this:

```
% .venv\Scripts\activate.bat
```

Once the virtualenv is activated, you can install the required dependencies.

```
$ pip install -r requirements.txt
```

At this point you can now synthesize the CloudFormation template for this code.

```
$ cdk synth
```

You can now begin exploring the source code, contained in the hello directory.
There is also a very trivial test included that can be run like this:

```
$ pytest
```

To add additional dependencies, for example other CDK libraries, just add to
your requirements.txt file and rerun the `pip install -r requirements.txt`
command.

## Useful commands

 * `cdk ls`          list all stacks in the app
 * `cdk synth`       emits the synthesized CloudFormation template
 * `cdk deploy`      deploy this stack to your default AWS account/region
 * `cdk diff`        compare deployed stack with current state
 * `cdk docs`        open CDK documentation

Enjoy!
