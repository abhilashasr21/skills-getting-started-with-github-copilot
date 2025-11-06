# storage_account module

Creates an Azure Storage Account and optional blob container.

Inputs:
- resource_group_name (required)
- location (required)
- storage_account_name (required; must be globally unique)
- account_tier, account_replication_type, enable_https_traffic_only, tags
- create_container (bool) and container_name (optional)

Outputs:
- storage_account_id
- primary_blob_endpoint
- container_id (if created)