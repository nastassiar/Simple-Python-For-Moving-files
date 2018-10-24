# Testing for ACI and Azure files

Files will start on a local machine
Create an Azure storage account either manually through the portal or with the Azure CLI
- Instructions specific to ACI: https://docs.microsoft.com/en-us/azure/container-instances/container-instances-volume-azure-files
- General instructions: https://docs.microsoft.com/en-us/azure/storage/files/storage-how-to-create-file-share
Use AzCopy to move files from local machine to the Azure Files you created previously
- https://docs.microsoft.com/en-us/azure/storage/common/storage-use-azcopy
Turn your Python application into a Docker Container
- https://runnable.com/docker/python/dockerize-your-python-application
Create an Azure Container registry to house the container that does work to the files on a mounted drive
- https://docs.microsoft.com/en-us/azure/container-registry/container-registry-get-started-portal
Use ACR to build container
- https://docs.microsoft.com/en-us/azure/container-registry/container-registry-tutorial-quick-task
Create ACI with that Azure File mounted as a drive
- https://docs.microsoft.com/en-us/azure/container-instances/container-instances-volume-azure-files
- https://docs.microsoft.com/en-us/azure/container-instances/container-instances-multi-container-group
Delete the container instance
- az container delete -g MyResourceGroup --name mycontainer
- https://docs.microsoft.com/en-us/cli/azure/container?view=azure-cli-latest#az-container-delete
- https://docs.microsoft.com/en-us/azure/container-instances/container-instances-quickstart
Check out the Files to see that they are changed!
- https://azure.microsoft.com/en-us/features/storage-explorer/