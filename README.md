# AWS VPC AUTOMATION

The project contains Ansible playbook to automate creation of AWS VPC infrastructure in order to develop machine learning solutions while ensuring data privacy.

## Getting Started
Clone the repository to your local machine:
```
git clone git@github.com:sapmlreseach/AWS_AnsiblePlaybook_MLResearch.git
```
### Prerequisites
Since it is an ansible script and uses awscli in order to set up components of VPC such as NAT gateway, you need to install following to your local machine:

```
pip install ansible
pip install boto
pip install awscli
```

### Configuring the playbook

1.Update the vars.yml file and change variable accordingly, depending on the use case of your organization.

2.Since ansible uses python interpreter, provide the right path to your python interpreter in local machine inside inventory file.



## Running the playbook

Switch to the directory where you cloned the repository and then enter the command:

```
ansible-playbook playbook.yml –i inventory –e @vars.yml
```
## Built With

* [Ansible](http://docs.ansible.com/ansible/latest/guide_aws.html) - Ansible automation tool
* [AWSCLI](https://aws.amazon.com/cli/) - Amazon Web Services command line interface


## Acknowledgments
1. https://blog.scottlowe.org/2015/11/21/using-ssh-bastion-host/

2. https://blog.scottlowe.org/2017/05/26/bastion-hosts-custom-ssh-configs/

3. http://tenmilesquare.com/using-ssh-through-a-bastion-host-transparently/

4. https://aws.amazon.com/vpc/
