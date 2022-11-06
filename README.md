# proedis/publish-nuget-package
Internal organization GitHub Action that could be used to Publish a NuGet Package on Private Proedis NuGet Registry

Usage:
```yml
    steps:
      - name: Publish NuGet Package on Proedis Registry
        uses: proedis/publish-nuget-package@v3
        with:
          project-folder: path/to/project
          project-file: Project.csproj
          registry-api-key: ........
```


### Properties
| Name | Required | Default | Description |
| :--- | :---:    | :---:   | :---        |
| `project-folder` | **true** | - | The folder that is containing the .csproj file |
| `project-file` | **true** | - | The project main file name, including the .csproj extension |
| `registry-api-key` | **true** | - | The ApiKey to use while pushing the package |
| `nuget-version` | *false* | `'latest'` | The NuGet Version to use |
| `dotnet-version` | *false* | `'6.x'` | The DotNet Version to use |
