# Provisioner
> Ansible playbooks to assist in setting up an Ubuntu system.
The playbooks are written with my personal setup in mind and
should be reviewed prior to running blindly.

> The provisioner will only run the tasks that have not been commented out in
`local.yml`. If you need to edit the tasks then it is recommended to use the third option in `Run Methods`

## Run Methods
> To use the provisioner, run any one of the following.
#### wget
```shell
sudo sh -c "$(wget https://raw.githubusercontent.com/otatski/provisioner/master/provision.sh -O -)"
```
#### curl
```shell
sudo sh -c "$(curl -fsSL https://raw.github.com/otatski/provisioner/master/provision.sh)" 
```
#### Manual
> 
```shell
git clone git@github.com:otatski/provisioner.git
cd provisioner
# Edit or add any tasks you wish to run.
ansible-playbook local.yml
```
