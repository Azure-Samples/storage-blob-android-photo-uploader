---
services: storage
platforms: android
author: pcibraro
---

# Azure Storage Service - Photo Uploader Sample for Android

This sample demostrates how to upload photo images from the gallery in Android into a Block Blob in Azure Storage. It shows different buttons for performing actions such as
selecting an image from the gallery, uploading an image to the blob storage or listing all the uploaded images.

Note: This is a project for Android Studio, which uses Gradle and references the Microsot Azure Storage Library for Android available in the Central Maven Repository. Also, it runs against the actual service, so it is highly recommended that you use a test container, 
as you will be creating and deleting actual blobs.

## Running this sample

1. Open the solution with Android Studio.
2. Open the ImageManager.java file and change the "[ACCOUNT_NAME]" and "[ACCOUNT_KEY]" in the storageConnectionString variable with account and key provided in the Azure Portal. 


|----------------|---------------------------|---------------|-------------------------|------------------|----------|                                                  **WARNING**
Only use Shared Key authentication for testing purposes! Your account name and account key, which give full read/write access to the associated Storage account, will be distributed to every person that downloads your app. This is not a good practice as you risk having your key compromised by untrusted clients. Please consult following documents to understand and use Shared Access Signatures instead. 

https://docs.microsoft.com/en-us/rest/api/storageservices/delegating-access-with-a-shared-access-signature
https://docs.microsoft.com/en-us/azure/storage/common/storage-dotnet-shared-access-signature-part-1
|----------------|---------------------------|---------------|-------------------------|------------------|---------|

## More information
- [What is a Storage Account](http://azure.microsoft.com/en-us/documentation/articles/storage-whatis-account/)
- [How to use Blob Storage from Android](https://github.com/Azure/azure-storage-android)
- [Blob Service Concepts](http://msdn.microsoft.com/en-us/library/dd179376.aspx)
- [Blob Service REST API](http://msdn.microsoft.com/en-us/library/dd135733.aspx)
