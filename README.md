# install-ocaml

# AWS EC2

AMI: Amazon Linux 2 LTS Candidate AMI 2017.12.0 (HVM)


if new image update & upgrade
```
sudo su
yum update -y && yum upgrade -y
yum install m4 patch ocaml -y
```

Install OPAM as per notes https://opam.ocaml.org/doc/Install.html
```
wget https://raw.github.com/ocaml/opam/master/shell/opam_installer.sh -O - | sh -s /usr/local/bin
```
get out of su and install rest with OPAM

```
exit

opam init

eval `opam config env`

opam switch

opam switch 4.06.1

opam install utop

```



