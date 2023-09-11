# Role listview

## Introduction

For years, Microsoft has used the so-called Listview role in Windows Explorer to display files and folders. Visually, there are several display types for the list:
* Details
* List
* Contents
* Symbols
* Tiles

## Examples for Listviews

### Microsoft Windows - File Explorer
Files can be arranged in different views for a better overview, preview of content or to expose different properties.

![Content View - Microsoft Windows](Windows/ContentView-Windows.png)

![Detail View - Microsoft Windows](Windows/DetailsView-Windows.png)

![Extra Large Symbols View - Microsoft Windows](Windows/ExtraLargeSymbolsView-Windows.png)

### Mac OSX - Finder

The functionalities covered by the finder are comparable to the ones offered by the Microsoft's file explorer.

![Coloumn View - Mac OSX - Finder](MacOSX/ColumnView-MacOSX.png)

![Gallery View - Mac OSX - Finder](MacOSX/GalleryView-MacOSX.png)

![List View - Mac OSX - Finder](MacOSX/ListView-MacOSX.png)

![Symbol View - Mac OSX - Finder](MacOSX/SymbolView-MacOSX.png)

### Fabasoft Cloud

As an example for an online platform where files and objects can be arranged in different views is Fabasofts Cloud. 

![Content View - Fabasoft Cloud](FabasoftCloud/ContentView-FabasoftCloud.png)

![Detail View - Fabasoft Cloud](FabasoftCloud/DetailView-FabasoftCloud.png)

![Preview View - Fabasoft Cloud](FabasoftCloud/PreviewView-FabasoftCloud.png)

![Thumbnail View - Fabasoft Cloud](FabasoftCloud/ThumbnailView-FabasoftCloud.png)

## The role listview

The real problem for AT users, especially screen reader users is, that without this role the list has to change the roles due to different display types from grid to treegrid (grouped list), to listbox (at the time the only possibility to display listview in list, content and tile type). The empty list is currently also a big problem.

As Sarah and Stefan already suggested, we also propose another complex role: **listview**.

The listview role should contain the following semantic properties:

### Accessibility children roles:
- listviewitem: basic listview object
  - feature: e.g: Values for filename, filesize, ...
- group: to group listviewitems
- featureheaders: container for featureheads (for detailed views)
  - featurehead: heading for a feature

### Listview attributes

- aria-listviewtype:
  - Allowed values: details | list | contents | tiles | symbols | thumbnails
- aria-multiselectable
- aria-readonly

## Next steps

- Filters: How can they be semanitcally connected to a list view?
- Keyboard navigation in different list view types

