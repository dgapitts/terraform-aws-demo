# terraform-aws-demo

## Other related projects

I have a couple of older vagrant centos7 training projects
* [vagrant-c7-terraform-docker](https://github.com/dgapitts/vagrant-c7-terraform-docker) following hashicorp training, a nice set of basic exercises 
* [vagrant-c7-aws-terraform-ansible](https://github.com/dgapitts/vagrant-c7-aws-terraform-ansible) which I was using for DevOpsDays Amsterdam training

I'm still working through the hashicorp training, but switching back to developing directly on my laptop, using the manual install of terraform (i.e. download binary and add to PATH).

## Working through hashicorp learn terraform demo for aws

### manual download of terraform for mac (amd64)

First I manually installed terraform on my mac, i.e. following 
* browse online https://www.terraform.io/downloads and then under MACOS BINARY DOWNLOAD I was able to select amd64 (choose arm64 if you're on the new M1/M2 processes)
* then following  https://learn.hashicorp.com/tutorials/terraform/install-cli "unpack and move to bin"

```
~/Downloads $ ls -l terraform_1.3.3_darwin_amd64.zip
-rw-r--r--@ 1 dave  staff  20843907 Oct 20 12:16 terraform_1.3.3_darwin_amd64.zip
~/Downloads $ unzip terraform_1.3.3_darwin_amd64.zip
Archive:  terraform_1.3.3_darwin_amd64.zip
  inflating: terraform
~/Downloads $ mv ~/Downloads/terraform /usr/local/bin/
```
* final test version
```
~/Downloads $ terraform --version
Terraform v1.3.3
on darwin_amd64
```
