# Satellites Guide

Satellites is an interactive table app for analysing satellites that are currently orbiting the Earth.

Data is sourced from the Union of Concerned Scientists (UCS) [UCS Satellite Database](https://www.ucsusa.org/resources/satellite-database)

![](satellites.gif)

## Features

- View aggregated statistics (summary)

- View individual records (details)

- Add and reorder columns

- Filter by double clicking

- Add cell bars

- Animate measure range

- Change the measure statistic

- Save all the above in up to eight custom views

## Control panel

Choosing the view, selecting columns, filtering and more is done with the control panel. If hidden, use the 'sun' switch to reveal (it is left of the eight 'planet' icon buttons).

![](satellites_control_panel.PNG)

## Table columns

The table has three types of columns:

- **Identifiers** are unique to each satellite
- **Factors** are words common to multiple satellites
- **Measures** are numbers and dates

Columns of the same type are positioned together in this order: Identifiers | Factors | Measures

## Views

**Summary** factor columns are on the left and aggregated measures are on the right side of the table.

**Details** identifier columns on the left, followed by factors and then measures on the right side of the table.

The summary view does not contain identifiers. The details view does not contain the count column.

## Show controls and save changes

The 'sun' switch hides/shows the concealable controls.
![](sun_reveal_control_panel.gif)

Eight circles (the 'planets') store eight sets of table views including summary/details selection, selected columns, filters, measure statistic and cell bar choices.

Saving is automatic, click the little circles to move between configurations.

## Select

Identifiers can only be seen in the 'Details' view. At least one factor is always shown. Measure columns are optional.

### Identifiers

To select identifier columns, click on '...more' (bottom right corner of controls) to reveal additional controls.

<img src="satellites_control_panel_more.PNG" width="100%">

Click insider the Identifiers selector and select the identifier columns you want added to the table.

<img src="satellites_select_identifier.PNG" width="50%">

Drag and drop the selected identifiers to reorder the columns in the table.

### Factors

Selecting factors is similar to identifiers, and columns can be reordered with drag and drop too.

<img src="satellites_select_factor.PNG" width="50%">

There are many factors to choose so scroll down and you'll find convenience commands that select all, inverse and clear the selection.

<img src="satellites_select_factor_command.PNG" width="50%">

Clearing will leave one factor remaining - it is a requirement of the table.

### Measures

Measures are selected similar to factors, columns reordered with drag and drop and convenience commands when you scroll down.

<img src="satellites_select_measure.PNG" width="50%">

When a selected measure is double clicked, it replaces the measure in the slider.

![](satellites_dblclick_measures.gif)

## Filter

Factors and measures can be filtered.

### Factors

Double click on a table cell in a factor column. It sends the filter to the factor filter selector.

![](satellites_factor_filter.gif)

Filters are removed with the keyboard delete key. They are saved in filter choices for later use - for example if you wanted to...

### Filter a factor column on more than one value

To have the same factor column filtered multiple times we'll have an example.

Let's say we want to view only military and commercial satellites.

1. filter on military
2. remove the filter, it will be stored for later
3. filter on civilian
4. add back the military filter

### Measures

The measure appearing in the slider label can be filtered by moving the slider knob. The slider is animated leading to some cool effects when combined with cell bars.

![](satellites_country_race.gif)

## Choose a measure statistic

There are four measure statistics to choose from:

- minimum
- average
- maximum
- standard deviation (measure of spread)

When showing standard deviation for dates, the unit of measure changes to days.

## Sort

Sort by clicking on the headers, shift-click to sort by multiple columns. This is standard reactable behaviour.

Saving the sort order on changes to the table is a custom feature of the app.

## Column descriptions

Hover over column headers to reveal descriptions.

<img src="satellites_header_definition.PNG" width="75%">

## Cell bars

Control which measure columns have cell bars using the additional '...more' control panel.

![](satellites_cell_bars.gif)

Cell bars implementation is a custom feature of the app in order to improve rendering speed.
