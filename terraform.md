## Terraform Commands Cheat Sheet

**Table of Contents:**
- [Terraform Commands Cheat Sheet](#terraform-commands-cheat-sheet)
  - [Terraform Basics](#terraform-basics)
  - [Working with Providers](#working-with-providers)
  - [Terraform Modules](#terraform-modules)
  - [Terraform State Management](#terraform-state-management)
  - [Working with Remote Backends](#working-with-remote-backends)
  - [Working with Variables](#working-with-variables)
  - [Advanced Commands](#advanced-commands)

### Terraform Basics

- `terraform init`: Initialize a Terraform working directory.
- `terraform plan`: Create an execution plan for Terraform changes.
- `terraform apply`: Apply Terraform changes to create or update infrastructure.
- `terraform destroy`: Destroy Terraform-managed infrastructure.
- `terraform validate`: Validate the configuration files in a Terraform directory.
- `terraform fmt`: Format Terraform configuration files to follow the standard style.
- `terraform show`: Show the current state or a saved plan.
- `terraform import <address> <id>`: Import existing resources into Terraform.
- `terraform output`: Show the outputs of the Terraform configuration.
- `terraform providers`: List all installed providers and their versions.
- `terraform refresh`: Update the state of Terraform-managed resources without modifying infrastructure.
- `terraform state`: Advanced state management and inspection commands.
- `terraform workspace`: Workspace management commands.
- `terraform version`: Show the installed version of Terraform.

### Working with Providers

- `terraform providers lock`: Lock installed provider versions to prevent automatic upgrades.
- `terraform providers mirror`: Copy provider plugins to a local mirror directory.
- `terraform providers schema`: Generate and display documentation for provider schemas.

### Terraform Modules

- `terraform get`: Download and install modules for the current configuration.
- `terraform module`: Module management and inspection commands.

### Terraform State Management

- `terraform state mv <address> <new-address>`: Move a resource within the Terraform state.
- `terraform state pull`: Fetch the current state from a remote backend.
- `terraform state push`: Upload the current state to a remote backend.
- `terraform state rm <address>`: Remove a resource from the Terraform state.
- `terraform state show`: Show the attributes of a resource in the Terraform state.

### Working with Remote Backends

- `terraform remote config`: Configure Terraform to use a remote backend.
- `terraform remote pull`: Fetch the current state from a remote backend.
- `terraform remote push`: Upload the current state to a remote backend.
- `terraform remote config -disable`: Disable remote state and revert to local state.

### Working with Variables

- `terraform apply -var 'key=value'`: Set a variable value inline during apply.
- `terraform apply -var-file=<file>`: Set variable values from a file during apply.
- `terraform plan -var 'key=value'`: Set a variable value inline during plan.
- `terraform plan -var-file=<file>`: Set variable values from a file during plan.
- `terraform refresh -var-file=<file>`: Set variable values from a file during refresh.
- `terraform show -var 'key=value'`: Set a variable value inline during show.
- `terraform show -var-file=<file>`: Set variable values from a file during show.

### Advanced Commands

- `terraform debug`: Debug output inspection commands.
- `terraform graph`: Generate a visual representation of the Terraform configuration graph.
- `terraform state pull`: Pull the current state and output as a JSON file.
- `terraform state push <filename>`: Update the state from a local JSON file.
- `terraform taint`: Manually mark a resource as tainted.
- `terraform untaint`: Manually clear the tainted state from a resource.
- `terraform validate -json`: Validate the configuration files in a Terraform directory and output the result in JSON format.
