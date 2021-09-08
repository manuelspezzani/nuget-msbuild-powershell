# nuget-msbuild-powershell
Sample package with an MSBuild .props file calling a powershell file

Just `nuget pack` the nuspec file and the resulting package will: 
- import the .props file to the target project
- on post-build it will the HelloWorld.ps1 file will be automatically invoked

Todo:
- [ ] test on a .NET Framework project (currently tested only on .NET Core)
- [ ] figure out if it's possible to remove the package version number on the .props file (worst case scenario: on build it can be updated automatically with the actual nuget version number)
