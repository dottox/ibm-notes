be# Create VPC using CLI

You'll need the IBM's CLI. You can install it [here](https://cloud.ibm.com/docs/cli?topic=cli-getting-started) via command line.

Otherwise, [here]() you can see the releases for the executable installer.

## 1. Login into your account

Use `ibmcloud login`, you'll have to do some steps.
> You can use the flag `--sso`for a single sign-on

## 2. Target the resource group

Now, you'll have to target your resource group. I think that this isn't necessarily if you're using a personal account (I can be wrong, clearly)

Use `ibmcloud target -g <resource_group_name>`
> Replace <resource_group_name> with your resource group's name. You can create one in the web UI or search for the CLI's command.

## 3. Create the VPC

Think about a name for the VPC, names don't have a global scope so you can use whatever you want.

In a shared account, it is a good practice to recall your resource group's name in the beginning of the VPC name. e.g `isuarez-vpc`

Use `ibmcloud is vpcc <vpc_name>`

> If this command doesn't work, you'll have to install a plugin to use the `is` command.
> To install the plugin, use `ibmcloud plugin install vpc-infrastructure`

## 4. Enjoy!

You created a VPC!
You can retrieve its info using `ibmcloud is vpc <vpc_name>` or delete it using `ibmcloud is vpcd <vpc_name>`

## Thank you!

> For improvements or fixes: Pull Request the repo, or contact me via Mail/Linkedin
