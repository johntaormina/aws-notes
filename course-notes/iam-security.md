## IAM (Identity and Access Management)

- All security
  - user -> groups -> roles
- Policies in IAM are written in JSON
- best to give users/roles *minimal* permissions they need to perform their job
- one IAM role per application

#### IAM Federation

- AWS login with company credentials
- Uses SAML standard (active directory)
- 

## Security Groups

- Act as a firewall (outside) to EC2 instances

- Regulate all control of networks - inbound and outbound

- Can be attached to mult instances

- Locked to region

- Good to maintain one separate security group for SSH access *

- Timeout - security group issue

- Connection Refused - security group worked, app error

- Can NOT reference DNS

- Can ref security group from another one

  

