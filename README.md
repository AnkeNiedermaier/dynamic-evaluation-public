# dynamic-evaluation-public
A PythonPart that tracks the objects of all currently loaded drawing files in ALLPLAN and dynamically evaluates attributes and quantities in tabular and graphical way in a separate window
## Installation
The PythonPart **DynamicEvaluation** can be installed directly from the Plugin Manager in ALLPLAN.

Alternatively, the corresponding ***.allep** package can be downloaded from the [release page](url of the release).\
 ***.allep** files are ALLPLAN internal setups that can be installed via drag and drop into the program window.

At least the version 2027 is needed to install and use the PythonPart.

## Installed PythonPart Scripts
If the installation was successfull, the PythonPart **DynamicEvaluation.pyp** can be found
in the ALLPLAN Library:
`Office` → `Allplan GmbH` → `DynamicEvaluation` → `DynamicEvaluation`

Additionaly it is also added to the ActionBar in a new created task area **Dynamic Evaluation** in the task **Dynamic Evaluation**.




## Workflow
In general, all installed PythonParts can be found in the Library palette, no matter if an additional ActionBar entry is created or not. They are started either with a **double-click** on the icon or per **Drag and Drop** into the viewport. This shows the corresponding Properties palette and executes the underlying skripts.

The evaluation as such is executed in a separate independend window that can be opened in cklicking the corresponding **Evaluation window start** button in the pallette.

> ⚠️IMPORTANT\
This is the only necessary step in the palette. Once the Evaluation window has been opened, the pallete can be closed and  continue in ALLPLAN as usual - opening new drawing files, changing projects, modifying objects ...



