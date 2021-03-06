# SAPUI5 IconList
![](https://img.shields.io/badge/SAPUI5-Library-blue)
![](https://badgen.net/badge/Version/1.0.0/green)

## Features
- SAPUI5 Standard Icon's
- Search based on Icon Names.

## Usage
IconList can be call as action event of Button and Input-ValueHelp controls.

#### Properties
Property                |Type           | Default Value   
-------------           | ------------- | -------------
title                   | string        | Icon List
noDataText              | string        | No Icon List
growing                 | boolean       | Icon List
rememberSelections      | boolean       | false
draggable               | boolean       | false
resizable               | boolean       | false
multiSelect             | boolean       | false
contentWidth            | string        | 
contentHeight           | string        | 
growingThreshold        | integer       | 60


#### Example
- ##### InputValue Help `(controller)`
```javascript
onValueHelpRequest: function(oEvent){
    let oIconList = new IconList();
    oIconList.open(oEvent);
},
```
- ##### InputValue Help `(view)`
```html
<Input
    type="Text"
    showValueHelp="true"
    valueHelpOnly="true"
    valueHelpRequest="onValueHelpRequest"
    class="sapUiSmallMarginBottom"
    width="15rem" />
```
- ##### Output
![Screenshot](output.png)



