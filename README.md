# PowerShell-module-templates

Store for module template resources created via plaster

## Use the Plaster module

Install-Module -Name plaster

Example for creating a module called MyModule:

```powershell
Invoke-Plaster  -DestinationPath C:\example\MyModule\ -Templatepath C:\example\
```

Where TemplatePath is the directory where the plasterManifest.xml file is located.
