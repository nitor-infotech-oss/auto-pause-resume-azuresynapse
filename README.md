# auto-pause-resume-azuresynapse
<h4>Objective:<h4>
<ul>
  <li>Primary objective of Auto Pause and Resume Azure Synapse DW is to save computation cost of Azure Synapse DW</li>
</ul>
<br/>
<h4>Key Features:</h4>
<ol>
  <li>Code will pause the azure synapse dw when dw is in idle state</li>
  <li>Also All the services which require Azure Synapse DW for analytics purpose will call resume pipeline to make DW online</li>
</ol>
<br/>
<h4>Implementation Steps:</h4>
<ul>
  <li>Import the ARM Template to your Azure Data Factory</li>
  <li>Configure Azure Synapse Linked Service</li>
  <li>Configure Azure Blob Storage Linked Service</li>
</ul>
<br/>
<h4>Configurations:</h4>
<ul>
  <li>Create Configuration File in configured Azure Storage Account which will be used for making API call to Azure DW to pause/resume/check status</li>
  <li>Add following details to config file: </li>
    <ol>
      <li>Add subscriptionid</li>
      <li>Add servername</li>
      <li>Add databasename</li>
      <li>Add resourcegroupname</li>
      <li>Add pausewaittime and resumewaittime</li>
    </ol>
</ul>
