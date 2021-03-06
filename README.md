## ec2grep - EC2 cli tool

### Install
Preferally for the default system interpreter instead of a virtualenv.

```bash
pip install git+https://github.com/bergundy/ec2grep
```

### Usage

##### ls
Basic usage, find by name tag, external / internal IP, DNS
```bash
ec2 ls my-hostname
```

Custom formatter (name, ip, extended)
```bash
ec2 ls --format=name my-hostname
```

##### ssh
Open an SSH session
```bash
ec2 ssh my-hostname
```

With arguments
```bash
ec2 ssh my-hostname -- w
```

##### custom region
```bash
ec2 --region us-west-2 ls my-hostname
```
