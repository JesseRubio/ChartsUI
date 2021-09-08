# SwiftUI Charts

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

Build custom charts with SwiftUI

<center>
<img src="Resources/customChart.png"/>
</center>

## Styles

### Line
<center>
<img src="Resources/lineChart.png"/>
</center>

```swift
Chart(data: [0.1, 0.3, 0.2, 0.5, 0.4, 0.9, 0.1])
    .chartStyle(
        LineChartStyle(.quadCurve, lineColor: .blue, lineWidth: 5)
    )
```

### Area
<center>
<img src="Resources/areaChart.png"/>
</center>

```swift
Chart(data: [0.1, 0.3, 0.2, 0.5, 0.4, 0.9, 0.1])
    .chartStyle(
        AreaChartStyle(.quadCurve, fill:
            LinearGradient(gradient: .init(colors: [Color.blue.opacity(0.2), Color.blue.opacity(0.05)]), startPoint: .top, endPoint: .bottom)
        )
    )
```

### Stacked Area

```swift
Chart(data: matrix)
    .chartStyle(
        StackedAreaChartStyle(.quadCurve, colors: [.yellow, .orange, .red])
    )
```

### Column
<center>
<img src="Resources/columnChart.png"/>
</center>

```swift
Chart(data: [0.1, 0.3, 0.2, 0.5, 0.4, 0.9, 0.1])
    .chartStyle(
        ColumnChartStyle(column: Capsule().foregroundColor(.green), spacing: 2)
    )
```

### Stacked Column

```swift
Chart(data: matrix)
    .chartStyle(
        StackedColumnChartStyle(spacing: 2, colors: [.yellow, .orange, .red])
    )
```

## Roadmap
-  Bar chart style

## Code Contributions
Feel free to contribute via fork/pull request to master branch. If you want to request a feature or report a bug please start a new issue.
