# LogicalisDevnet  

## NEP@L & NSO Integration

## NSO Service: Deployment ACLs
  
In order to provide NSO with two highly required or demanded features like CI/CD nd workflow manager, we made the decision to integrate NEP@L and NSO using Ansible as a DSL (Domain specfic language) and NSO APIs. While NSO remain te tools that access the network, NEP@L allow NSO user and developers to have CI/CD pipelines and execute Uses Case via the workflow manager interface.

Below, three files that are part of the mentioned service that shows de integration

Files  
Service Model.yaml: Source of True of the service  
play_config_template_acl.yaml: playbook that configure into NSO the templates defined in the Source of True  
play_config_acl.yaml: playbook that tells NSO to impact or configure the devices with template previously defined in NSO

## Execution

As mentiones above, each artifact called playbook, is linked to a task in the workflow manager on NEP@L. Every task the workflow executes, correspond to an action NSO must execute as part of the Use Case definition. The Use Case is then executed from NEP@L workflow manager instead of NSO CML or GUI interface

## Pre requisities

 from the Software pre requisites stand point, an NSO 4.X and higher instance and NEP@L 2.0 instance are both nedded in order the integration to work. Also, the Use Case must alredy exist (modeled and configured) on NSO

## Integration Diagram

An integration diagram file is now part of the project
