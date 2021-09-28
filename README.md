![](https://img.shields.io/badge/STATUS-NOT%20CURRENTLY%20MAINTAINED-red.svg?longCache=true&style=flat)

# Important Notice
This public repository is read-only and no longer maintained. For the latest sample code repositories, visit the [SAP Samples](https://github.com/SAP-samples) organization.

# AWS VPC AUTOMATION

## Description:
The project contains Ansible playbook to automate creation of AWS VPC infrastructure in order to develop machine learning solutions while ensuring data privacy.

## Getting Started
Clone the repository to your local machine:
```
git clone git@github.com:sapmlreseach/AWS_AnsiblePlaybook_MLResearch.git
```
## Requirements
Since it is an ansible script and uses awscli in order to set up components of VPC such as NAT gateway, you need to install following to your local machine:

```
pip install -r requirements.txt
```

## Download and Installation

1.Update the vars.yml file and change variable accordingly, depending on the use case of your organization.

2.Since ansible uses python interpreter, provide the right path to your python interpreter in local machine inside inventory file.


## Running the playbook

Switch to the directory where you cloned the repository and then enter the command:

```
ansible-playbook playbook.yml –e @vars.yml
```
## Built With

* [Ansible](http://docs.ansible.com/ansible/latest/guide_aws.html) - Ansible automation tool
* [AWSCLI](https://aws.amazon.com/cli/) - Amazon Web Services command line interface

## Known Issues
No issues known


## How to obtain support
This project is provided "as-is" and any bug reports are not guaranteed to be fixed.


## Acknowledgments
1. https://blog.scottlowe.org/2015/11/21/using-ssh-bastion-host/

2. https://blog.scottlowe.org/2017/05/26/bastion-hosts-custom-ssh-configs/

3. http://tenmilesquare.com/using-ssh-through-a-bastion-host-transparently/

4. https://aws.amazon.com/vpc/

## License

This project is licensed under SAP Sample Code License Agreement except as noted otherwise in the [LICENSE file](LICENSE.md).
