# typicon-swift
Use the [typicon font](http://www.typicons.com) in your Swift projects.

## Usage

### Setup
* Add the .swift file and the .ttf file to your Xcode project.
* Go to the Build Phases tab of your project and add the ttf file to the 'Copy Bundle Resources' phase.
* Go to the Info tab of your project. Under 'Custom iOS Target Properties', add the 'Fonts provided by application' array entry if it does not already exist. Add a new item and set the value to `typicons.ttf`.

### Using the font
* Creating a UIFont:

    ```
UIFont.typiconFontOfSize(50)
```
* Setting the font of a control:

    ```
myButton.titleLabel?.font = UIFont.typiconFontOfSize:50
```
* Setting text content of a control to an icon:

    ```
myButton.titleLabel?.text = String.typiconStringForIconName("arrow-right-thick")
```
* To find the identifier for an icon, go to <http://typicons.com> and hover over an icon - the name of the icon will be displayed.
