# blut_aws_tf_minecraft fargate instructions

## Build image with non-auto download files copied over
```bash

cd build
docker build . -t jardo_minecraft
```



## Terraform
```bash
# env vars set NOT RECOMMMENDED
export AWS_ACCESS_KEY_ID=your_aws_access_key
export AWS_SECRET_ACCESS_KEY=your_aws_secret_access_key

terraform init
terraform apply
```

## References
- https://hub.docker.com/r/itzg/minecraft-server/tags
- https://docker-minecraft-server.readthedocs.io/en/latest/types-and-platforms/mod-platforms/auto-curseforge/#api-key
- https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli
- https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html 
- https://banhawy.medium.com/3-ways-to-configure-terraform-to-use-your-aws-account-fb00a08ded5
- https://github.com/tfutils/tfenv


# Client instructions
- Install CurseForge: https://www.curseforge.com/download/app
- Install ATM9 with the zip file 
- This should make a new entry under the 'My Modpacks' tab in your CurseForge app, click play on the top left :p
- This should bring up your MC launcher, use java edition
- The screen may look red and scary, don't be afraid Andi
- Once launcher has loaded click MULTIPLAYER
- Select direct connect and put IP without port (I'll provide from AWS console)
- done :tada: