# PowerShell-module-templates

Store for module template resources created via plaster

## Use the Plaster module

Install-Module -Name plaster

Example for creating a module called MyModule:

```powershell
Invoke-Plaster  -DestinationPath C:\example\MyModule\ -Templatepath C:\example\
```

Where TemplatePath is the directory where the plasterManifest.xml file is located.


```powershell

$plasterParams = @{
    TemplatePath = 'C:\git\PowerShell-module-templates\ModuleTemplate\'
    DestinationPath = 'C:\git\DotNetCoreReleaseTool\'
    Fullname = 'Matthew Davis'
    ModuleName = 'DotNetCoreReleaseTool'
    ModuleDesc = 'Commands to work with the latest release of DotNet Core from the DotNet repo'
    Version = '0.0.1'
    PowerShellVersion = '5.1'
}

Invoke-Plaster $plasterParams
```