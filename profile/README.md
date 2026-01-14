<div align="center">
    <img width="128" src="https://raw.githubusercontent.com/phellams/phellams-general-resources/main/logos/phellams/dist/png/phellams-logo-512x512.png" alt="Phellams Logo">
    <h1>Phellams</h1>
    <code>[P]owers[HELL][A]uto[M]ation[S]</code> </br></br>
    <p>Houses PowerShell Modules,  <b>Scripts</b>,  <b>Libraries</b>,  <b>Tools</b>,  <b>Dotnet Libraries</b>,  <b>Dotnet (AOT) cli  apps</b>,</p>
</div>

---


##  ❇️  **PowerShell**

Modules are split into 3 categories:
 - **SMEP**(*Single Module Entry Point*) - Modules with a single `.psm1` file and uses the `Invoke-ModuleName` to control the module, and can simply be imported with `using module` and if packaged with `.psd1` `Import-Module`
 - **MMEP**(*Multi Module Entry Point*) - Modules with multiple .psm1 files in hirarchcal structure.
 - **DMMEP**(*Defined Multi Module Entry Point*) - Module that follow the same princal and **MMEP** but actions are defined, eg `invoke-ModuleNameAction`, `invoke-ModuleNameAction`, `invoke-ModuleNameAction`, and are contrained to set defined number of cmdlets that are exported, the inverse of **SMEP** actions.

 
 **SEMP**: 
  - `Invoke-ModuleName -> action(create|update|remove|import|export)`
    > Usally in `$moduleroot\modulename.psm1`

 **MMEP**: 
  - `Get-CmdletCreate` 
  - `Get-CmdletUpdate`
  - `Get-CmdletRemove`
  - `Get-CmdletImport`
  - `Get-CmdletExport`
    > Usally in `$moduleroot\cmdlets\*.psm1`



Utility modules (**SMEP**) are distributed <code>PowerShellGallery</code> and <code>GitLab Packages</code> nuget packages as well as being self contained in a single .psm1 file.

Smaller libraries, tools, and scripts clone the repository and manually import the module, see module readme for details.

##  ❇️  Dotnet(c#)

**Dotnet Core CLI Apps** and **Dotnet 10 (AOT) CLI Apps** are distributed as <code>Nuget</code> <code>GitLab Packages</code> nuget packages.

## **Respositories**

### Phellams Powershell Respositories:
#  👉   <a href="https://community.chocolatey.org/profiles/sgkens"><img src="https://img.shields.io/badge/Chocolatey-Repo-Brown?style=for-the-badge&logoSize=auto&labelColor=%23693C5E&color=%23007C80"></a> <a href="https://www.powershellgallery.com/profiles/sgkens"><img src="https://img.shields.io/badge/PSGallery-Repo-Brown?style=for-the-badge&logoSize=auto&labelColor=%234B0082&color=%23007C80"></a> <a href="https://gitlab.com/phellams"><img src="https://img.shields.io/badge/GitLab-Repo-Brown?style=for-the-badge&logoSize=auto&labelColor=%234B0082&color=%23007C80"></a>


### Phellams .NET Nuget Respositories:

### Phellams Mirrors

![Mirror][gitHubMirror]

### **Notable Finished Projects**:

|Status|Project|Repository|Description|Language|
|---|---|---|---|---|
| ✔️|![phellams-logo][phellams-logo-link] | [**Phellams Automator**](https://gitlab.com/phellams/phellams-automator) |*Docker Container to build and publish modules to the PowerShell Gallery, choco, gitlab packages and publish release via gitlab*|`PowerShell`|
| ✔️|![phellams-logo][phellams-logo-link] | [**Automator Devops**](https://gitlab.com/phellams/phellams-profile) |*GitLab Workflow templat and release script to be used with phellams-automator docker image*|`PowerShell`|
| ✔️|![commitfusion-logo][commitfusion-logo-link] | [**CommitFusion**](https://gitlab.com/phellams/commitfusion) |*Conventional Commit Helper*|`PowerShell`|
| ✔️|![fastfsc-logo][fastfsc-logo-link] | [**FastFSC**](https://gitlab.com/phellams/fastfsc)|*A high-performance PowerShell module for calculating folder sizes using inline C# code.*|`PowerShell`, `C#`|
| ✔️|![magicgester-logo][magicgester-logo-link] | [**MagicGester**](https://gitlab.com/phellams/magicgester)|*Uses InkScape and magick to output set x.x pixel images(**.png** **.jpg** **.ico**) from SVGs*|`PowerShell`|
| ✔️|![psshields-logo][psshields-logo-link] | [**PsShields**](https://gitlab.com/phellams/psshields)|*PowerShell Module to create shields.io badges*|`PowerShell`|
| ✔️|![pwsl-logo][pwsl-logo-link] | [**Pwsl**](https://gitlab.com/phellams/pwsl)|*PowerShell Module to interacting with the Windows Subsystem for Linux*|`PowerShell`|
| ✔️|![phwriter-logo][phwriter-logo-link] | [**Phwriter**](https://gitlab.com/phellams/phwriter)|*PowerShell Module to general linux man page style help*|`PowerShell`|
| ✔️|![zypline-logo][zypline-logo-link] | [**Zypline**](https://gitlab.com/phellams/zypline)| *PowerShell Module for advanced file and folder searching with configuration management.*|`PowerShell`|


#### **🚧 WIP Project Tracker**:

|Status|Project|Repository|Description|Language|
|---|---|---|---|---|
| 🚧|![auspex-logo][auspex-logo-link] | [**Auspex**](https://gitlab.com/phellams/auspex)| *A robust engine for performing Deep CRUD (Create, Read, Update, Delete) and Array Manipulation (Push/Pull) on complex PowerShell data structures.* |`PowerShell`|
| 🚧|![gitpare-logo][gitpare-logo-link] | [**GitPare**](https://gitlab.com/phellams/gitpare)| *PowerShell Module to interact with gitpare*|`PowerShell`|
| 🚧|![glvigor-logo][glvigor-logo-link] | [**Glvigor**](https://gitlab.com/phellams/glvigor)| *PowerShell Module to interact gitlab api to perform crud operations on a number of gitlab endpoints*|`PowerShell`|

## 📑 Licences

Modules are released under the:
[MIT License](https://github.com/phellams/phellams/blob/main/LICENSE)

[**Phellams-General-Resources**](https://github.com/phellams/Phellams-General-Resources) Such as Icons and logos are released under the [Creative Commons Zero v1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/deed.en) `/svgrepo` are added under there original [Creative Commons Zero v1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/deed.en)

<div align="center">
  <img src="https://raw.githubusercontent.com/phellams/.github/refs/heads/main/images/userstats.svg" />
</div>

[gitHubMirror]: https://img.shields.io/badge/GitHub-Mirror-Brown?style=for-the-badge&logoSize=auto&labelColor=%23000&color=%23008000
[magicgester-logo-link]: https://raw.githubusercontent.com/phellams/phellams-general-resources/main/logos/phellams/dist/png/phellams-logo-32x32.png
[fastfsc-logo-link]: https://raw.githubusercontent.com/phellams/phellams-general-resources/main/logos/phellams/dist/png/phellams-logo-32x32.png
[phellams-logo-link]: https://raw.githubusercontent.com/phellams/phellams-general-resources/main/logos/phellams/dist/png/phellams-logo-32x32.png
[commitfusion-logo-link]: https://raw.githubusercontent.com/phellams/phellams-general-resources/main/logos/commitfusion/dist/png/commitfusion-logo-32x32.png
[psshields-logo-link]: https://raw.githubusercontent.com/phellams/phellams-general-resources/main/logos/psshields/dist/png/psshields-32x32.png
[pwsl-logo-link]: https://raw.githubusercontent.com/phellams/phellams-general-resources/main/logos/pwsl/dist/png/pwsl-32x32.png
[phwriter-logo-link]: https://raw.githubusercontent.com/phellams/phellams-general-resources/main/logos/phwriter/dist/png/phwriter-logo-32x32.png
[zypline-logo-link]: https://raw.githubusercontent.com/phellams/phellams-general-resources/main/logos/zypline/dist/png/zypline-logo-32x32.png
[auspex-logo-link]: https://raw.githubusercontent.com/phellams/phellams-general-resources/main/logos/auspex/dist/png/auspex-32x32.png
[gitpare-logo-link]: https://raw.githubusercontent.com/phellams/phellams-general-resources/main/logos/gitpare/dist/png/gitpare-32x32.png
[glvigor-logo-link]: https://raw.githubusercontent.com/phellams/phellams-general-resources/main/logos/glvigor/dist/png/glvigor-32x32.png



