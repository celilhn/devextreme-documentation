---
id: dxPolarChart.Options.valueAxis.minorTickInterval
acceptValues: 'day' | 'hour' | 'millisecond' | 'minute' | 'month' | 'quarter' | 'second' | 'week' | 'year'
type: Number | Object | String
inherits: VizTimeInterval
---
---
##### shortDescription
Specifies the interval between [minor ticks](/concepts/05%20UI%20Components/Chart/20%20Axes/07%20Axis%20Ticks.md '/Documentation/Guide/UI_Components/Chart/Axes/Axis_Ticks/').

---
To divide a lengthy chart axis into shorter segments, major and minor ticks are used. Between each pair of neighboring major ticks, several minor ticks reside. Minor ticks are required when major ticks are far from each other. To set a custom minor tick interval, use the **minorTickInterval** property. If this property is not set, minor ticks are arranged automatically.

In case your axis displays numbers, assign a numeric value to this property. If the axis displays dates, assign one of the predefined string values. To set the interval to several days, hours, etc., assign an object with the corresponding field specified (**days**, **hours** or another field). Note that this object must contain only one of the fields described in this section.

[note]The **minorTickInterval** property can be applied to a *[continuous](/api-reference/10%20UI%20Components/dxPolarChart/1%20Configuration/valueAxis/type.md '/Documentation/ApiReference/UI_Components/dxPolarChart/Configuration/valueAxis/#type')* axis only. For logarithmic axes, use the [minorTickCount](/api-reference/10%20UI%20Components/dxPolarChart/1%20Configuration/valueAxis/minorTickCount.md '/Documentation/ApiReference/UI_Components/dxPolarChart/Configuration/valueAxis/#minorTickCount') property.

When using the UI component as an <a href="https://docs.devexpress.com/DevExtremeAspNetMvc/400943/devextreme-aspnet-mvc-controls" target="_blank">ASP.NET MVC 5 Control</a> or a <a href="https://docs.devexpress.com/AspNetCore/400263/aspnet-core-controls#devextreme-based-aspnet-core-controls" target="_blank">DevExtreme-Based ASP.NET Core Control</a>, specify this property using the `VizTimeInterval` enum. This enum accepts the same values, but they start with an upper-case letter, for example, *'day'* becomes `Day`.