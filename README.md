# How to deploy your first Aspire (.NET9) application in Azure cloud

## 1. Prerrequisites

### 1.1. Install Visual Studio 2022 Preview for .NET 9

https://visualstudio.microsoft.com/vs/preview/

![image](https://github.com/user-attachments/assets/c7f8d6c2-29af-4147-8f94-7d6e05ab3a74)

### 1.2. Install .NET 9 SDK 

https://dotnet.microsoft.com/en-us/download/dotnet/9.0

![image](https://github.com/user-attachments/assets/4300fcae-135c-43b0-b407-07e701ccb590)

### 1.3. Install .NET Aspire

https://learn.microsoft.com/en-us/dotnet/aspire/fundamentals/setup-tooling?tabs=windows&pivots=visual-studio

![image](https://github.com/user-attachments/assets/9fd5ee49-7065-4e8e-b206-224e97390641)

or 

```
dotnet workload install aspire
```

And verify the installation

```
dotnet workload list
```

![image](https://github.com/user-attachments/assets/49d6c103-3fa9-4cba-a5b8-737f6d7ceaf9)

### 1.4. Install .NET Aspire 9

https://learn.microsoft.com/en-us/dotnet/aspire/whats-new/dotnet-aspire-9-release-candidate-1?tabs=windows&pivots=visual-studio

```
dotnet new install Aspire.ProjectTemplates::9.0.0-rc.1.24511.1
```

or 

```
dotnet new install Aspire.ProjectTemplates::9.0.0-rc.1.24511.1 --force
```

### 1.5. Install Docker Desktop

https://www.docker.com/products/docker-desktop/

![image](https://github.com/user-attachments/assets/ce5589c5-d425-4676-b081-4bdec4bf5323)

![image](https://github.com/user-attachments/assets/3518c90e-bd4c-4b50-bd65-30babd4829ba)

### 1.6 Install Azure Developer CLI

https://learn.microsoft.com/en-us/azure/developer/azure-developer-cli/install-azd

To install with **PowerShell** run this command

```powershell
powershell -ex AllSigned -c "Invoke-RestMethod 'https://aka.ms/install-azd.ps1' | Invoke-Expression"
```

For intalling with **choco** run his command

```
choco install azd
```

Verify the installation running this command

```
azd version
```

**NOTE**: How to install **chocolatey**

https://chocolatey.org/install

## 2. How to create the Aspire .NET 9 application with Visual Studio 2022

We run Visual Studio and we create a new project

We select the project template

We input the project name and location

We review the projec files and folder structure

## 3. How to deploy the application in Azure

We select the Aspire Host project as the StartUp project

We right click on the Aspire Host project and select the option Open in the Solution Explorer

We reun the command **azd init**

![image](https://github.com/user-attachments/assets/60cc4eb4-b407-4446-9503-6fdff230e8f0)

![image](https://github.com/user-attachments/assets/ce6385fa-0cb7-4e88-b23d-6efdcd43c141)

![image](https://github.com/user-attachments/assets/d0dc9a71-50b0-44a4-8360-13fffbc9bfde)

![image](https://github.com/user-attachments/assets/107f3880-47c3-44a4-a48d-224d052009fe)

![image](https://github.com/user-attachments/assets/fc88c32a-848c-4001-a9ac-88dda01e7ada)

![image](https://github.com/user-attachments/assets/026374e9-f00e-4e1c-9fc4-d6a6b727720b)

![image](https://github.com/user-attachments/assets/5e50a168-c846-4d92-9510-a309b4526c21)


