# Day 0 - AWS and Server Setup

### Tasks accomplished
- Set up AWS account.
- Set up MFA.
- Set up IAM user.
- Set up a Zero-Spend Budget (Notifies if a spend exceeds $0.01).
- Familiarizzed myself with [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html).

#### AWS CLI install and update instructions:
1. `sudo apt remove awscli`
2. Download and install AWS CLI in one command: `curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install`
3. Confirm installation and version: `aws --version`

#### Confiure AWS CLI:
1. Download access keys for the IAM account or user:
- Security credentials/IAM >> Create Access Keys
2. Configure the AWS CLI in the terminal:
- `aws configure`

#### Environment Variables (Env Variables)- Optional:
Save the credentials then use them when setting up AWS CLI
```bash
export AWS_ACCESS_KEY_ID=EXAMPLE
export AWS_SECRET_ACCESS_KEY=EXAMPLE
export AWS_DEFAULT_REGION=us-west-2
```
Credentials are lost after every restart meaning you need to reconfigure.

#### CLI Basics
- Command structure: `aws <command> <subcommand> [options and parameters]`

### Tasks accomplished(continued)
- Launched an EC2. 
    - First, generate a keypair. EC2 >> Network & Security >> Key pairs
    - [Create, display, and delete Amazon EC2 key pairs](https://docs.aws.amazon.com/cli/latest/userguide/cli-services-ec2-keypairs.html)
    - [Launch, list, and terminate EC2 instances](https://docs.aws.amazon.com/cli/latest/userguide/cli-services-ec2-instances.html)
    - List all instances: `aws ec2 describe-instances`
    - Add a tag to your instance: `aws ec2 create-tags --resources i-5203422c(resource ID) --tags Key=specify Name,Value=Specify MyInstance`
- Connected to instance via SSH:

**NB:** Ensure that an inbound rule for port 22 is present.

    `ssh -i keyname.pem ec2-user@ipaddress`

