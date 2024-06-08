![Static Badge](https://img.shields.io/badge/Template%20Version-V0.01-pink) ![Static Badge](https://img.shields.io/badge/Node-GoogleDrive-f8f8f8) ![Static Badge](https://img.shields.io/badge/Node-GoogleDriveOAuth2Api-f8f8f8) ![Static Badge](https://img.shields.io/badge/Node-SplitInBatches-f8f8f8) ![Static Badge](https://img.shields.io/badge/Node-ManualTrigger-f8f8f8) ![Static Badge](https://img.shields.io/badge/Node-Code-f8f8f8) ![Static Badge](https://img.shields.io/badge/Node-NoOp-f8f8f8) ![Static Badge](https://img.shields.io/badge/Node-templates-f8f8f8)
![Static Badge](https://cdn.statically.io/gh/Automations-Project/n8n-templates/main/src/img/covers/n8n-bulk-automated-google-drive-files-sharing-and-direct-download-link-generation/idNEgS9h8q.jpeg)

# Bulk Automated Google Drive Files Sharing and Direct Download Link Generation

This N8N workflow automates the process of sharing files from Google Drive. It includes OAuth2 authentication, batch processing, public link generation, and access status modification for efficient file handling. Suitable for users seeking to streamline their Google Drive file sharing process. sutiable for bulk actions, tested on 4.2K files folder working like charm.

![xeL6OxvdLi.png](fileId:725)

### How It Works

1. **Initialize Workflow**: The process begins with a Manual Trigger, allowing the user to start the workflow at their convenience.
2. **Folder ID Specification**: A 'Set Folder ID' node where the user can enter the desired Google Drive Folder ID.
3. **List Files from Google Drive**: The 'Google Drive' node lists all files within the specified folder using OAuth2 authentication.
4. **Batch Processing**: The 'Loop Over Items' node processes the files in batches for efficiency.
5. **Generate Public Links**: The 'Generate Download Links' node creates downloadable links for each file.
6. **Change File Access**: The 'Change Status' node alters the file status to make them publicly accessible.
7. **Merge and Output**: A 'Merge' node consolidates the data, preparing it for further actions or output.

### Set Up Steps

* **Estimated Time**: The setup should take approximately 10-15 minutes.
* **Initial Setup**: You'll need to provide OAuth2 credentials for Google Drive and specify a folder ID.
* **Customization**: Adjust the batch size and file access permissions according to your needs.
* **Detailed Descriptions**: For specific configuration details, refer to the sticky notes within the workflow.

### Example Item output
```JSON
{
"link": "https://drive.google.com/u/3/uc?id=1hojqPfXchNTY8YRTNkxSo-8txK9re-V4&export=download&confirm=t&authuser=0",
"name": "firefox_rNjA0ybKu7.png",
"kind": "drive#permission",
"id": "anyoneWithLink",
"type": "anyone",
"role": "reader",
"allowFileDiscovery": false
}
```
You can store the output data with any data store node you want, for example save them into Excel Sheet or Airtable etc...
```
Keywords: n8n workflow, Google Drive integration, file sharing automation, batch file processing, public link generation, OAuth2 authentication, workflow automation
```


# Stats
[![N8N Creator Profile - Nskha](https://cdn.statically.io/gh/Automations-Project/n8n-templates/main/stats.min.svg)](https://n8n.io/creators/nskha)