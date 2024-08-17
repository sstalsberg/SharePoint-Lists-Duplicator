# SharePoint Lists Duplicator
This PowerShell script is designed to copy list items from one SharePoint list to another, including handling image fields. The script connects to the specified SharePoint site, retrieves items from the source list, and then duplicates them into the target list, ensuring that image fields are correctly processed and copied.

## Prerequisites

Before running the script, ensure that you have PnP PowerShell Module: 
```
Install-Module -Name PnP.PowerShell
```
## Script Parameters
The script uses several parameters that need to be configured before execution:

•	$SiteURL: The URL of your SharePoint site.
•	$SourceListId: The ID or title of the source SharePoint list from which items will be copied.
•	$TargetListId: The ID or title of the target SharePoint list where items will be copied to.
•	$ImageField: The internal name of the image field in the source list that needs to be copied.
•	$DownloadFolderPath: A local folder path where images will be temporarily downloaded before being uploaded to the target list.

## Usage
1.	Configure the Parameters: Modify the script to include your SharePoint site URL, list IDs, and other necessary parameters.
2.	Run the Script: Execute the script in PowerShell to start the copying process.

 ## Notes
•	Ensure that the $DownloadFolderPath directory is writable and has enough space to temporarily store images during the process.
•	The script currently assumes that image fields are stored in JSON format within the SharePoint list. Ensure that your image fields are correctly configured in this format.
