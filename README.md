# TurtleUi
# By Intrer#0421
# Documention by MiniBeta666

## Load Lib
```lua
local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/miroeramaa/TurtleLib/main/TurtleUiLib.lua"))()
```
## Window
```lua
local window = library:Window("Window")
```
## Button
```lua
window:Button("Button name", function()
   print("pressed button")
end)
```
## Toggle
```lua
window:Toggle("Example toggle", true, function(bool)
    print(bool) -- bool is true or false depending on the state of the toggle
end)
```
## Color Picker
```lua
window:ColorPicker("Color Picker", Color3.fromRGB(255, 255, 255), function(color)
   print(color)
end)
```
## Slider
```lua
window:Slider("Example Slider",0,100,20, function(value)
   print(value)
end)
```
## Label
```lua
window:Label("Credits to Intrer#0421", Color3.fromRGB(127, 143, 166))
```
## TextBox
```lua
window:Box("Walkspeed", function(text, focuslost)
   if focuslost then
   print(text)
   end
end)
```
## DropDown
```lua
local dropdown = window:Dropdown("Example dropdown", {"Button 1", "Button 2", "Third button"}, function(name)
   print(name)
end)
```
## Add button dropdown
```lua
dropdown:Button("New button")
```
## Remove button dropdown
```lua
dropdown:Remove("Button")
```
## Toggle ui keybind
```lua
library:Keybind("P")
```
