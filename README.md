Remove all Blobs (including Snapshots) from One Windows Azure Storage Account
=============================================================================

            

[Windows Azure Scripting Center](http://www.windowsazure.com/en-us/documentation/scripts) |
[Get Started with Windows Azure PowerShell](http://go.microsoft.com/fwlink/?linkid=320929&clcid=0x409) |
[Windows Azure Data Management Scripts](http://www.windowsazure.com/en-us/documentation/scripts/index/?solution=data-management&service=all)

Description

Removes blobs from blob storage containers. The script will enumerate through all containers and remove the blobs, maintaining the existence of the container. If you want to remove the containers, then you can include the RemoveContainer switch. This will
 be faster than removing the individual blobs in the container but will require you to recreate the container if you wish to use it again.


Prior to removing all blobs in a container or the container itself, the user is prompted to confirm the operation. This enables you to apply the operation to some (but not all) containers. If you include the Force switch, then all blobs will be removed from
 all containers and all containers will be removed if the RemoveContainer switch is applied.


**Note:** This script requires an Azure Storage Account to run. The storage account can be specified by setting the subscription configuration. For example,


Set-AzureSubscription -SubscriptionName 'MySubscription' -CurrentStorageAccount 'MyStorageAccount'

Example
 
Scenario
You want to remove all blobs from a container or set of containers. Or, you want to remove containers and the blobs within the container.
Requirements

  *  PowerShell Version 3.0 
  *  Windows Azure PowerShell 0.6.18 
See Also

  *  [Set-AzureSubscription](http://msdn.microsoft.com/en-us/library/windowsazure/dn408531.aspx)

  *  [Windows Azure Data Management Scripts](http://www.windowsazure.com/en-us/documentation/scripts/index/?solution=data-management&service=all)

Script Content

The content of the script is reproduced below

 

        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
