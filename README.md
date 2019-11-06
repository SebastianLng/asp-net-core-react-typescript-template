# ASP.NET Core 3 React Typescript Template

Here is how you create a project with a default React Typescript app:

1. Create an ASP.NET Core 3 project with the React Template in Visual Studio.
2. Remove the Content of the "ClientApp" Folder.
3. Create a react app with [create-react-app](https://create-react-app.dev/docs/adding-typescript/) in an arbitrary folder somewhere else. 
  For example:
  
```sh
  npx create-react-app myapp --typescript
```
4. Copy the content of the created Typescript React app into the "ClientApp"-Folder.
5. Visual Studio should promt you to install the Typescript NuGet Package. If it does not, you can add the reference manually:

```XML
<PackageReference Include="Microsoft.TypeScript.MSBuild" Version="3.7.2">
    <PrivateAssets>all</PrivateAssets>
    <IncludeAssets>runtime; build; native; contentfiles; analyzers; buildtransitive</IncludeAssets>
</PackageReference>
```

5. You now have a working, debuggable default react app with Typescript running with ASP.NET Core.