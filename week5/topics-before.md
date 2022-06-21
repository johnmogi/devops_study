## Infrastructure as Code

[What is Infrastructure as Code]
{{ Infrastructure as Code (IaC) is the managing and provisioning of infrastructure through code instead of through manual processes. With IaC, configuration files are created that contain your infrastructure specifications, which makes it easier to edit and distribute configurations}}

iaac is a modern approach to handle IT, instead of manual "toggling"
we impliment changes using pre-built configuration files.

[Why use Infrastructure as Code]
{{ Faster speed and consistency: The goal of IaC is to make things faster by eliminating manual processes and eliminating the slack in the process. A code-based approach makes it easier to get more done in less time. No need to wait on the IT Admin to manually complete the task at hand before he can get to the next one.}}

not only this approach makes chang monitoring and cI CID easier, it also saves time by shortenting the memory curve on ui.

[Main Tools for Infrastructure as Code]
{{ Terraform. Terraform is one of the most popular IaC tools in the market. ...
AWS CloudFormation. ...
Azure Resource Manager. ...
Google Cloud Deployment Manager. ...
Pulumi. ...
Ansible. ...
Chef. ...
Puppet. }}
ansible | chef | peppet || terraform (best for building stage 1)

## Terraform

[Terraform Architecture]
{{ HashiCorp Terraform is an open source infrastructure as code (IaC) software tool that allows DevOps engineers to programmatically provision the physical resources an application requires to run. Infrastructure as code is an IT practice that manages an application's underlying IT infrastructure through programming. }}
-declerative
deployments are made in a idopetent manner (looking at final result)

[Terraform Configuration Language (HCL)]
{{ HashiCorp Configuration Language (HCL) is a unique configuration language. It was designed to be used with HashiCorp tools, notably Terraform, but HCL has expanded as a more general configuration language. It's visually similar to JSON with additional data structures and capabilities built-in. }}
json / python approach and very shortcut manner

[Terraform CLI Usage]
{{ Use the Terraform Command Line Interface (CLI) to manage infrastructure, and interact with Terraform state, providers, configuration files, and Terraform Cloud.}}

[Terraform Providers]
{{ Terraform can provision infrastructure across public cloud providers such as Amazon Web Services (AWS), Azure, Google Cloud, and DigitalOcean, as well as private cloud and virtualization platforms such as OpenStack and VMWare.}}
azure, gcp, aws - each provider has it's own set of rules.

[Terraform Variables]
{{ Variables in Terraform are a great way to define centrally controlled reusable values. The information in Terraform variables is saved independently from the deployment plans, which makes the values easy to read and edit from a single file.}}

[Terraform Outputs]
{{ Terraform outputs allow you to share data between Terraform workspaces, and with other tools and automation. Outputs are also the only way to share data from a child module to your configuration's root module.}}
cli maniests once apply has been succseful - you can also chain them forward.

[Terraform Backends]
{{Backends define where Terraform's state snapshots are stored. A given Terraform configuration can either specify a backend, integrate with Terraform Cloud, or do neither and default to storing state locally.}}

[Terraform Modules]
{{ A Terraform module allows you to create logical abstraction on the top of some resource set. In other words, a module allows you to group resources together and reuse this group later, possibly many times.9}}
