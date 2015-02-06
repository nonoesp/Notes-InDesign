# Notes-InDesign

Useful notes for InDesign.

## Table of Contents

* Folder Structure
* Styles
* Document Templates
* Workflows

## Folder Structure

**InDesign/**

Contains the current presentation.

**PDF/**

Contains the current PDF document, and old version in Archive/

**Archive/**

Contains old versions of the InDesign document

### Styles

### Paragraph Styles

#### Case Scenarios

* Type/ (text, blockquote, footnote)
* Annotations/ (comment-printed, comment-not-printed, dimension, label)
* Layout/ (header, footer)

### Headers

Different levels of headers for each document.

* H1
* H2
* H3
* H4
* H5
* H6
* Text
* Labels
* Title
* Subtitle

### Object Styles

#### Case Scenarios

* Tags
* Line Styles

### Character Styles

#### Case Scenarios
* Bold
* Italic
* Underline

### Document Types

* Report
* Presentation

## Workflows

### Set Text Variables with JSON

Document templates with multiple text variables can be quickly filled with data using JSON objects.

```JavaScript

var settings = {title: 'Title',
		            subtitle: 'Your Subtitle Here'};

app.activeDocument.textVariables.item("Title").variableOptions.contents = settings.title;
app.activeDocument.textVariables.item("Subtitle").variableOptions.contents = settings.subtitle;
```
