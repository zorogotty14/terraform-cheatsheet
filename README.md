# Terraform Cheatsheet

## **Terraform Overview**
Terraform is an Infrastructure as Code (IaC) tool that allows you to define and manage cloud resources using configuration files.

---

## **Terraform Installation & Version Check**
```sh
terraform --version            # Check installed Terraform version
terraform -help                # Get help with Terraform commands
```

---

## **Initializing Terraform**
```sh
terraform init                 # Initialize Terraform in the working directory
terraform init -upgrade        # Upgrade provider plugins
```

---

## **Planning & Applying Configuration**
```sh
terraform plan                 # Show execution plan without applying changes
terraform apply                # Apply Terraform configuration
terraform apply -auto-approve  # Apply without confirmation prompt
```

---

## **Destroying Resources**
```sh
terraform destroy              # Destroy all resources managed by Terraform
terraform destroy -auto-approve # Destroy without confirmation prompt
```

---

## **Managing Terraform State**
```sh
terraform state list           # List all resources in the state file
terraform state show <resource> # Show details of a specific resource
terraform state rm <resource>  # Remove resource from state (without deleting it)
terraform taint <resource>     # Mark a resource for recreation
terraform refresh              # Sync state with real-world resources
```

---

## **Working with Modules**
```sh
terraform get                  # Download and update modules
terraform init -reconfigure    # Reinitialize Terraform modules
```

---

## **Terraform Outputs**
```sh
terraform output               # Display output values from Terraform state
terraform output <name>        # Display a specific output variable
```

---

## **Terraform Variables**
```sh
terraform plan -var='name=value'  # Pass a variable value inline
terraform apply -var-file=<file>  # Pass a variable file
```

---

## **Formatting & Validation**
```sh
terraform fmt                   # Format Terraform configuration files
terraform validate              # Validate Terraform configuration files
```

---

## **Locking & Unlocking State**
```sh
terraform force-unlock <lock_id> # Force unlock a Terraform state file
```

---

## **Remote Backend Configuration**
```sh
terraform backend config <args>   # Configure Terraform backend
```

---

## **Useful Terraform Resources**
- [Terraform Official Docs](https://developer.hashicorp.com/terraform/docs)
- [Terraform Registry](https://registry.terraform.io/)
- [Terraform Best Practices](https://developer.hashicorp.com/terraform/tutorials)

---

This cheatsheet provides a quick reference for working with Terraform efficiently. Let me know if you have any suggestions or improvements!

