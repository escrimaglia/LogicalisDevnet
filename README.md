# LogicalisDevnet  

## NEP@L & NSO Integration

## NSO Service: Deployment ACLs
  
In order to provide NSO with two highly required or demanded features like CI/CD nd workflow manager, we made the decision to integrate NEP@L and NSO using Ansible as a DSL (Domain specfic language) and NSO APIs. While NSO remain te tools that access the network, NEP@L allow NSO user and developers to have CI/CD pipelines and execute Uses Case via the workflow manager interface.

Below, three files that are part of the mentioned service that shows de integration

Files  
Service Model.yaml: Source of True of the service  
play_config_template_acl.yaml: playbook that configure into NSO the templates defined in the Source of True  
play_config_acl.yaml: playbook that tells NSO to impact or configure the devices with template previously defined in NSO
