# Azure Terraform module deployment structure

This repository layout provides an Azure-specific Terraform module development and deployment structure.

Highlights:
- modules/: reusable Azure-focused Terraform modules (storage_account, virtual_network)
- examples/: root examples that consume the modules for testing
- .github/workflows/: CI to run terraform fmt/init/validate (includes Azure login step)
- scripts/: helper scripts for validation and formatting
- backend.tf.example: example Azure Storage backend configuration for remote state

Use the examples/azure-simple root module to test locally (configure Azure credentials first).