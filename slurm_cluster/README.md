# Install


## edit hosts for setup cluster

```bash
linux:~/slurm_cluster # cp hosts.example hosts
linux:~/slurm_cluster # vi hosts
```


## check all package config/var/file

```bash
linux:~/slurm_cluster # ls */{vars,files}/*
```


## run ansible to setup cluster

```bash
linux:~/slurm_cluster # ansible-playbook site.yml -v
```


---

# Note

the playbook only test on centos 7.6

