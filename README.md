# Cisco ACI Configuration: Firewall Integration ACI and PBR with same BD

Nexus as Code configuration example to setup a service graph with PBR with firewall legs in the same BD as the client and server

See [Nexus as Code](https://developer.cisco.com/docs/nexus-as-code/) for the full documentation.

## Quick Start

- `git clone https://github.com/conmurphy/aci-pbr-same-bd.git`
- `cd aci-pbr-same-bd`
- Update `terraform.tfvars` with your environments details or add the variables as environmental variables
  - `export TF_VAR_aci_url=https://my-apic-url.local`
- `terraform init`
- `terraform plan`
- `terraform apply`

# Notes

- The Terraform code will deploy two tenants with all EPGs, BDs, Contracts, and Service Graphs
- It will not configure the L3Domain, AAEP, or VLAN pool
- It is assumed that the ASA and VMware have already been setup
- This scenario is configured to use an ASAv running on UCS connected through Fabric Interconnects

## License

This project is licensed to you under the terms of the [Cisco Sample
Code License](./LICENSE).


