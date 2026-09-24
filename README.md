# How to Remove Comma-Separated Indexed Category Axis Labels in Syncfusion Blazor Chart

## Overview

This sample demonstrates how to customize indexed category axis labels in Syncfusion [Blazor Charts](https://www.syncfusion.com/blazor-components/blazor-charts). When multiple series are displayed with an indexed category axis, the chart can generate axis labels that contain multiple category values separated by commas. The sample handles the `OnAxisLabelRender` event and modifies the label text so that only the first category value is displayed on the primary X-axis.

This approach helps improve chart readability when multiple series contain different category values but a simplified axis presentation is preferred.

## Key Features

- Uses the `SfChart` component to render chart data.
- Configures the primary X-axis with `IsIndexed="true"`.
- Sets the axis `ValueType` to `Category`.
- Uses the `ChartEvents` component and the `OnAxisLabelRender` event.
- Receives label information through `AxisLabelRenderEventArgs`.
- Identifies the primary X-axis through `args.Axis.Name`.
- Customizes axis label text through the `args.Text` property.
- Renders multiple column series using `ChartSeries`.
- Binds chart data using the `DataSource`, `XName`, and `YName` properties.
- Uses `ChartSeriesType.Column` for series visualization.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download the repository.
2. Open the project file from the `RemoveComma` project folder.
3. Restore NuGet packages when prompted.
4. Build the project.
5. Run the application using **Ctrl+F5**.

**Visual Studio Code**

1. Open the repository folder in Visual Studio Code.
2. Open the integrated terminal.
3. Navigate to the project directory.

```bash
cd RemoveComma
dotnet restore
dotnet run
```

4. Open the local URL displayed in the console after the application starts.

## Project Structure

`Pages/Index.razor` - Hosts the Syncfusion Blazor Chart sample, configures the indexed category axis, defines chart series, supplies sample data, and handles axis label customization through `OnAxisLabelRender`.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Refer to the Syncfusion Blazor Chart documentation: https://help.syncfusion.com/chart-sdk/blazor/charts/getting-started

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.