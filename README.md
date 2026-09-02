# Dynamic Evaluation
The **Dynamic Evaluation** tracks the objects of all currently loaded drawing files in ALLPLAN and dynamically evaluates attributes and quantities in tabular and graphical way in a separate window

In this it offers an easy to catch overview of the model data and a direct feedback of the impact of changes on the project
 
## Installation
The PythonPart **DynamicEvaluation** can be installed directly from the Plugin Manager in ALLPLAN.

Alternatively, the corresponding ***.allep** package can be downloaded from the [release page](https://github.com/AnkeNiedermaier/dynamic-evaluation-public/releases).\
 ***.allep** files are ALLPLAN internal setups that can be installed via drag and drop into the program window.

At least the version 2027 is needed to install and use the PythonPart.

## Installed PythonPart Scripts
If the installation was successfull, the PythonPart **DynamicEvaluation.pyp** can be found
in the ALLPLAN Library:
`Office` → `Allplan GmbH` → `DynamicEvaluation` → `DynamicEvaluation`

Additionaly it is also added to the ActionBar in a new created task area **Dynamic Evaluation** in the task **Dynamic Evaluation**.




## Workflow
In general, all installed PythonParts can be found in the Library palette, no matter if an additional ActionBar entry is created or not. They are started either with a **double-click** on the icon or per **Drag and Drop** into the viewport. This shows the corresponding Properties palette and executes the underlying skripts.

The evaluation as such runs in a separate independend window that can be opened in clicking the corresponding **Evaluation window start** button in the palette.

> ⚠️IMPORTANT\
This is the only necessary step in the palette. Once the Evaluation window has been opened, the palette can be closed and work in ALLPLAN can continue as usual - opening new drawing files, changing projects, modifying objects ...

## General usage
The window is divided into two corresponding parts, a **table** at the left and a **diagram** at the right side, showing attributes and quantities of the current loaded model data.

The attribute to be focussed on and the quantity to be calculated is selected with the **Key attribute** and **Quantity attribute** Pulldown in the Toolbar. Besides choosing an existing entry, for example **Material** and **Volume** any ALLPLAN attribute - also userdefined ones - can be added to the Pulldown in typing in the attribute name.

Whereas the table structure as such is fixed, the kind of diagram is choosen from the **Diagram type** Pulldown in the toolbar.\
For **Bar** and **Column** diagrams also a second sorting criteria can be used to structure the data, for example the **Piece** of **Objects** for the different **Materials**. When the corresponding Checkbox is ticked another Pulldown for the **Sorting attribute** is available that can be used in the same way like **Key** and **Quantity** in selecting or typing in the desired attribute of interest.

> ⚠️IMPORTANT\
If Key and Sorting attribute are identical or the Sorting attribute is set to **None** it will be ignored. As soon as the Diagram type **Ring** or **Pie** is choosen, the Sorting attribute is disabled as it is currently not supported by this types

The accurate quantity value of an attribute is not only listed in the table, but also shown when hoovering over a slice or bar in the diagram

## Tools and menus

The **Menu** bar at the top of the window offers several possibilities to customize the diagram apperance and export, save or load content.

### File menu

Besides the life tracking that updates automatically during changes, it is also possible to save a static snapshot of the current loaded data for later review. Therefor the **File** menu contains the two options
- **Save as Snapshot** to write the current data into a file
- **Open Snapshot file** to load a previous saved state into the Evaluation window. It can then be explored in the same way as the dynamic one in defining Key or Quantity attribute, changing the diagram type ....

> ⚠️IMPORTANT\
Once a static file is loaded, the dynamic update is paused. At the same time the **Restart dynamic update!** button becomes enabled and if it is clicked the life synchronisation will start again

- **Print content** to print both the diagram and the table

### Export menu

Besides printing the **Export** menu offers additional possibilities to save the content in other forms for further use
- export the table as **Excel file**
- save the diagram as **bitmap**

### Diagram menu

To controll the behaviour and appearance of the diagram the menu offers several options that could be checked or unchecked
- show the bars or slices in **Gradient** color
- place a **Legend** at the right side of the diagram
- show **Grid lines** in Bar and Column diagrams
- **Label** the single slices in Pie and Ring diagramm
- **Animation** to redraw the diagram with every action


### Info menu

A direct link to the documentation is provided within the **Help** option, whereas the **About** entry shows information about the current installed version

When closing the Evaluation window, the object tracking is stopped immediately. It can be restarted in opening the window again as described at the beginning.

