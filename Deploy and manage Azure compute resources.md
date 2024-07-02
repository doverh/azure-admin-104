# Deploy and manage Azure compute resources

## Automate deployment of resources by using Azure Resource Manager (ARM) templates or Bicep files

Resource Manager allow you to create, update and delete resources on Azure. Access Controls locks and tags allow you to secure and organize resources after deployment.

Resources manages allow you to group resouces which makes easy to deploy them in a given environment.

Template will define what resources are available in a deployment.

### Benefits

- Improve consistency.
- Help express complex deployments. Templates enable you to deploy multiple resources in the correct order.
- Templates reduce manual, error-prone tasks.
- Templates are code.
- Templates promote reuse.
- Templates are linkable. You can link Resource Manager templates together to make the templates themselves modular.
- Templates simplify orchestration.

{
    "*$schema": "http://schema.management.​azure.com/schemas/2019-04-01/deploymentTemplate.json#",​
    "*contentVersion": "",​
    "parameters": {},​
    "variables": {},​
    "functions": [],​
    "*resources": [],​
    "outputs": {}​
} * required

### Parameter section

"parameters": {
    "<parameter-name>" : {
        "type" : "<type-of-parameter-value>",
        "defaultValue": "<default-value-of-parameter>",
        "allowedValues": [ "<array-of-allowed-values>" ],
        "minValue": <minimum-value-for-int>,
        "maxValue": <maximum-value-for-int>,
        "minLength": <minimum-length-for-string-or-array>,
        "maxLength": <maximum-length-for-string-or-array-parameters>,
        "metadata": {
        "description": "<description-of-the parameter>"
        }
    }
}
256 is the limit of parameters.

Azure Bicep is a domain-specific language (DSL) that uses declarative syntax to deploy Azure resources. It provides concise syntax, reliable type safety, and support for code reuse.

You can use Bicep instead of JSON to develop your Azure Resource Manager templates (ARM templates).

When Deployment with same configurations runs a second time no action is taken.

- You can *deploy, manage, and monitor all the resources for your solution as a group*.
Resources can be deployed to any new or existing resource group. Deployment of resources to a resource group becomes a job where you can track the template execution.
- You can repeatedly *deploy your solution throughout the development lifecycle*
- You can manage your infrastructure through *declarative templates* rather than scripts.
- You can *define the Ídependencies between resources* so they're deployed in the correct order.
- You can apply access control to all services in your resource group because *Role-Based Access Control (RBAC)* is natively integrated into the management platform.
- You can *apply tags to resources to logically organize all the resources in your subscription*.
- You can *clarify your organization's billing by viewing costs for a group of resources sharing the same tag*.

Interpret an Azure Resource Manager template or a Bicep file

Modify an existing Azure Resource Manager template

Modify an existing Bicep file

Deploy resources by using an Azure Resource Manager template or a Bicep file

Export a deployment as an Azure Resource Manager template or convert an Azure 

Resource Manager template to a Bicep file

## Create and configure virtual machines

Create a virtual machine

Configure Azure Disk Encryption

Move a virtual machine to another resource group, subscription, or region

Manage virtual machine sizes

Manage virtual machine disks

Deploy virtual machines to availability zones and availability sets

Deploy and configure an Azure Virtual Machine Scale Sets

## Provision and manage containers in the Azure portal

Create and manage an Azure container registry

Provision a container by using Azure Container Instances

Provision a container by using Azure Container Apps

Manage sizing and scaling for containers, including Azure Container Instances and Azure Container Apps

## Create and configure Azure App Service

Provision an App Service plan

Configure scaling for an App Service plan

Create an App Service

Configure certificates and Transport Layer Security (TLS) for an App Service

Map an existing custom DNS name to an App Service

Configure backup for an App Service

Configure networking settings for an App Service

Configure deployment slots for an App Service