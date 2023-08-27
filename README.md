# AzureVS2022VM
Create VS 2022 VM in Azure using a template

*** This approach is a workaround as the current portal is hosed and will not allow users with VS subscriptions (Pro or Enterprise) to create a VM image (that has inbuilt VS 2022).
***
***

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
