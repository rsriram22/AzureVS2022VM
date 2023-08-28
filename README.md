# Azure Visual Studio 2022 VM

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Ftackiertangent%2FAzureVS2022VM%2Fmain%2Ftemplate.json)


## How to create VS 2022 VM in Azure using a template (for Visual Studio users with a subscription)

***
***
  This approach is a workaround as the Azure portal is hosed and will not allow users with VS subscriptions (Pro or Enterprise) to create a VM image (that has 
  inbuilt VS 2022).
***
***

## Background:

I ran into the same error as described here - https://learn.microsoft.com/en-us/answers/questions/1305434/how-to-solve-this-subscription-spending-limit-issu
(Apparently, it's not resolved since June 14)

### Error:
    "The virtual machine requires a subscription without any spending limit or temporary payment method set. Use a different subscription or update your subscription"

![Error](https://learn-attachment.microsoft.com/api/attachments/06b51a16-0d6e-4eff-a4d3-0725f48e389f?platform=QnA)

## Workaround:

Steps to create a VM from template:

1. Open portal (portal.azure.com)
2. Create a new 'Template Spec' ('Templates' are being retired soon)
3. Enter basic info
4. Click 'Edit Template' at bottom
5. Copy/Paste the content from 'template.json' file from this repo
6. Save
7. Click 'Deploy'
8. Enter the info you know (resource group,location etc)
9. Other details, look at the parameters.json file and you get the idea of what-to-fill-in. The placeholders are in <> tags.
10. Thats it!
