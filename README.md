# Seamlessly Load Data from Different Data Sources into Blazor Charts

## Overview

This sample demonstrates how to bind and visualize data from multiple sources using the Syncfusion [Blazor Charts](https://www.syncfusion.com/blazor-components/blazor-charts) component. The application showcases several real-world data-binding scenarios including strongly typed collections, observable collections, dynamic objects, JSON files, remote Web APIs, and SQL Server databases.

Each page focuses on a specific data source implementation and illustrates how the Syncfusion Chart component can consume different data structures while maintaining a consistent visualization experience. This sample serves as a practical reference for developers who need to display business data from various sources in Blazor applications.

## Key Features

- Uses Syncfusion Blazor Chart component to render data-driven visualizations.
- Demonstrates chart data binding from multiple data sources.
- Shows how Blazor pages can provide data to chart series.
- Includes reusable application structure for integrating additional datasets.
- Uses strongly typed data models stored within the project.
- Renders data using the `SfChart` component with Material 3 theme support.
- Demonstrates data binding using strongly typed `List<Patient>` collections through the `ChartSeries.DataSource` property.
- Shows dynamic data binding using `List<ExpandoObject>` with `XName` and `YName` field mapping.
- Includes examples of both local and remote data retrieval patterns for Blazor applications.

## Prerequisites

- Visual Studio 2022 or Visual Studio Code
- .NET SDK compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download the repository.
2. Open the solution file:

   `ChartDatasourceApp.sln`

3. Restore all NuGet packages.
4. Set the startup project to:

   `ChartDatasourceApp`

5. Build the solution.
6. Run the project using `Ctrl+F5`.

**Visual Studio Code**

1. Open the repository folder in Visual Studio Code.
2. Open the integrated terminal.
3. Navigate to the project directory containing `ChartDatasourceApp.csproj`.

4. Restore packages:

```bash
dotnet restore
```

5. Run the application:

```bash
dotnet run
```

6. Open the local URL displayed in the application output.

## Project Structure

`ChartDatasourceApp.sln` - Visual Studio solution file.

`ChartDatasourceApp.csproj` - Blazor project definition and NuGet package references.

`Program.cs` - Application startup and service registration.

`App.razor` - Root Razor component.

`_Imports.razor` - Shared namespace imports.

`Pages/Index.razor` - Default homepage displaying a Syncfusion chart bound to a strongly typed `List<Patient>` collection.

`Pages/ListDataChart.razor` - Demonstrates chart binding using a custom `List<Patient>` data source.

`Pages/ObservableDataChart.razor` - Demonstrates chart binding using `ObservableCollection<PatientDetail>`.

`Pages/ExpandoDataChart.razor` - Demonstrates dynamic chart binding using `List<ExpandoObject>`.

`Pages/JsonDataChart.razor` - Loads chart data from `data/oildata.json` using `HttpClient.GetFromJsonAsync()`.

`Pages/RemoteDataChart.razor` - Demonstrates remote data binding using `SfDataManager` with `WebApiAdaptor`.

`Pages/SQLDataChart.razor` - Retrieves chart data from SQL Server and renders literacy rate statistics.

`Pages/FetchData.razor` - Default Blazor weather forecast page demonstrating service-based data retrieval.

`appsettings.json` - Application configuration settings.

`appsettings.Development.json` - Development environment configuration settings.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Refer to the official Syncfusion Blazor Charts documentation: https://help.syncfusion.com/chart-sdk/blazor/charts/getting-started

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.