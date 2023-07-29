## Azure 104 BC = 2216012201 

### Powershell

``Install-Module -Name Az -Repository PSGallery -Force``

``Connect-AzAccount``                                      

``echo $PSHOME``

``$PSVersionTable``

``Install-Module -Name Az -Repository PSGallery -Force``

``Connect-AzAccount``

``Get-AzLocation``

``Get-AzLocation | Format-List -Property Location, DisplayName``

``Get-AzRessourceGroup``

``Remove-AzResourceGroup -Name TestRG2 -Force``

### CLI

https://learn.microsoft.com/en-us/cli/azure/what-is-azure-cli

``az login``

``az group list``

``az account list``
  
``az account list -o table``
  
### Virtual Machine
https://learn.microsoft.com/en-us/azure/virtual-machines/overview

### LAB - Create A VM

### Disks
https://learn.microsoft.com/en-us/azure/virtual-machines/managed-disks-overview


### VM Scale Sets

https://learn.microsoft.com/en-us/azure/virtual-machine-scale-sets/overview

### Availibility Set

https://learn.microsoft.com/en-us/azure/virtual-machines/availability-set-overview

- Fault domain
- Update domain

### custom images
https://learn.microsoft.com/en-us/azure/virtual-machines/linux/tutorial-custom-images


## Azure Storage
https://learn.microsoft.com/en-us/azure/storage/common/storage-introduction

### Listing the container

http://127.0.0.1:10000/devstoreaccount1?comp=list	

``` XML
<EnumerationResults ContainerName="https://demo223344.blob.core.windows.net/demo">
<Blobs>
<Blob>
<Name>notes.md</Name>
<Url>https://demo223344.blob.core.windows.net/demo/notes.md</Url>
<LastModified>Sat, 29 Jul 2023 13:49:40 GMT</LastModified>
<Etag>0x8DB903AA7C1B9B7</Etag>
<Size>3903</Size>
<ContentType>application/octet-stream</ContentType>
<ContentEncoding/>
<ContentLanguage/>
</Blob>
<Blob>
<Name>sample.html</Name>
<Url>https://demo223344.blob.core.windows.net/demo/sample.html</Url>
<LastModified>Sat, 29 Jul 2023 13:48:02 GMT</LastModified>
<Etag>0x8DB903A6D87734F</Etag>
<Size>222</Size>
<ContentType>text/html</ContentType>
<ContentEncoding/>
<ContentLanguage/>
</Blob>
</Blobs>
<NextMarker/>
</EnumerationResults>
```

https://learn.microsoft.com/en-us/rest/api/storageservices/list-containers2?tabs=azure-ad

Example Error for invalid Page Blob :
Page blob size must be aligned to a 512-byte boundary. The following files are invalid: Module-5-Assignment-2.pdf


## Youtube
EyDea - 104 Exam Q's Style

https://www.youtube.com/watch?v=wYUhumwOGrM&list=PLA_CqAntXBh4DPIYCcplBWLjT3AYl1822


John Savil
Full master Cram

https://www.youtube.com/watch?v=VOod_VNgdJk&list=PLlVtbbG169nGlGPWs9xaLKT1KfwqREHbs




## From Azure Slack
Latest Update Notes
The July 24 2023 exam update had several changes. The following are some important notes about these changes.
Azure AD is now weighted higher (was 15-20%, now 20-25%)
Azure AD has changed name to Entra ID (but no features have changed)
All Azure AD content is still valid
Virtual Networking reduced (was 20-25%, now 15-20%)
Bicep templates have been added
Some content is no longer listed on the exam outline, but is still included in this course because it may still remain in some exams. It is recommended that you do not skip this for the time being. This includes:
Import/Export jobs
Azure Kubernetes Service (including scaling, networking, etc)
