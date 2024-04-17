# RedZ UI V2
This documentation is for RedZ UI V2 Credit To REDZ

## Booting the RedZ UI V2 UI Library
```lua
loadstring(game:HttpGet(("https://raw.githubusercontent.com/REDzHUB/LibraryV2/main/redzLib")))()
```




## Creating a RedZ UI V2 UI Window
```lua
MakeWindow({
  Hub = {
    Title = "REDz HUB",
    Animation = "by : redz9999"
  },
  Key = {
    KeySystem = false,
    Title = "Key System",
    Description = "",
    KeyLink = "",
    Keys = {"1234"},
    Notifi = {
      Notifications = true,
      CorrectKey = "Running the Script...",
      Incorrectkey = "The key is incorrect",
      CopyKeyLink = "Copied to Clipboard"
    }
  }
})

--[[
  Hub = {
    Title = "REDz HUB"
    Animation = "by : redz9999"
  },
  Key = {
    KeySystem =
    Title = "Key System"
    Description = ""
    KeyLink = ""
    Keys = {"1234"}
    Notifi = {
      Notifications = true
      CorrectKey = "Running the Script..."
      Incorrectkey = "The key is incorrect"
      CopyKeyLink = "Copied to Clipboard"
    }
  }
]]
```

## MiniMize Button
```lua
MinimizeButton({
  Image = "",
  Size = {40, 40},
  Color = Color3.fromRGB(10, 10, 10),
  Corner = true,
  Stroke = false,
  StrokeColor = Color3.fromRGB(255, 0, 0)
})

--[[
  Image = ""
  Size = {40, 40}
  Color = Color3.fromRGB(10, 10, 10)
  Corner = true
  Stroke = false
  StrokeColor = Color3.fromRGB(255, 0, 0)
]]
```

## Creating a Tab
```lua
local Main = MakeTab({Name = "Main"})

--[[
  Name = "Main" <string> Tab name
]]
```

## Creating a Notify
```lua
MakeNotifi({
  Title = "REDz HUB",
  Text = "Notification Testing",
  Time = 5
})

--[[
  Title = "REDz HUB"
  Text = "Notification Testing"
  Time = 5 <number> notification time
]]
```

## Creating a Section
```lua
local section = AddSection(Main, {"Test"})
--[[
  {"Test"} <table> window name
]]
```

## Creating a Set Section
```lua
SetSection(section, "HI")
```

## Creating a Button
```lua
AddButton(Main, {
  Name = "Button Testing",
  Callback = function()
    
  end
})

--[[
  Name = "Button Testing"
  Callback = function()
    -- function of your button
  end
]]
```

## Creating a Toggle
```lua
local Toggle = AddToggle(Main, {
  Name = "Toggle Test",
  Default = false,
  Callback = function(Value)
    
  end
})

--[[
  Name = "Toggle Test"
  Default = false
  Callback = function(Value)
    -- function of your checkbox
  end
]]
```

## Creating a Mobile Toggle
```lua
local MobileToggle = AddMobileToggle({
  Name = "Toggle",
  Visible = true,
  Callback = function(Value)
    
  end
})

MobileToggle.Visible = (false/true)

--[[
  Name = "Toggle"
  Visible = false
  Callback = function()
    -- check box function
  end
]]
```

## Creating a Slider
```lua
local Slider = AddSlider(Main, {
  Name = "Slider Test",
  MinValue = 10,
  MaxValue = 100,
  Default = 25,
  Increase = 1,
  Callback = function(Value)
    
  end
})

--[[
  Name = "Slider teste"
  MinValue = 10
  MaxValue = 100
  Default = 25
  Increase = 1
  Callback = function(Value)
    slider function
  end
]]
```

## Creating a Keybind
```lua
AddKeybind(Main, {
  Name = "Keybind Test",
  KeyCode = "E",
  Default = false,
  Callback = function(Value)
    
  end
})

--[[
  Name = "Keybind test"
  KeyCode = "E"
  Default = false
  Callback = function(Value)
    -- keyboard shortcut function
  end
]]
```

## Creating a TextBox
```lua
AddTextBox(Main, {
  Name = "TextBox Test",
  Default = "redz",
  PlaceholderText = "hub",
  ClearText = true,
  Callback = function(Value)
    
  end
})

--[[
  Name = "TextBox Test"
  Default = "redz"
  PlaceholderText = "hub"
  ClearText = true
  Callback = function(Value)
    -- text box function
  end
]]
```

## Creating a Dropdown
```lua
local Dropdown = AddDropdown(Main, {
  Name = "Dropdown Test",
  Options = {"1", "2", "3"},
  Default = "2",
  Callback = function(Value)
    
  end
})

--[[
  Name = "Dropdown teste" <string> dropdown menu name
  Options = {"1", "2", "3"}
  Default = "2"
  Callback = function(Value)
    -- dropdown menu function
  end
]]
```

## Creating a Color Picker
```lua
AddColorPicker(Main, {
  Name = "Color Picker Test",
  Default = Color3.fromRGB(255, 255, 0),
  Callback = function(Value)
    
  end
})

--[[
  Name = "Color picker teste" <string> Color sector name
  Default = Color3.fromRGB(255, 255, 0)
  Callback = function(Value)
    -- color sector function
  end
]]
```

## Creating a Paragraph
```lua
local Paragraph = AddParagraph(Main, {"Paragraph Test", "hello"})

--[[
  Paragraph Name
  description of the Paragraph
]]
```
## Creating a Set Paragraph 
```lua
SetParagraph(Paragraph, {"Paragraph", ":>"})

--[[
  Paragraph Name
  Paragraph description
]]
```

## Creating a Label
```lua
local Label = AddTextLabel(Main, "AutoFarm")

--[[
  Text
]]
```

## Creating a Set Label
```lua
SetLabel(Label, "HI")

--[[
  Text
]]
```

## Creating a Image Label
```lua
local Image = AddImageLabel(Main, {
  Name = "Cool Image",
  Image = "rbxassetid://"
})

--[[
  Name = "Cool Image"
  Image = "rbxassetid://"
]]
```

## Set Image
```lua
SetImage(Image, "rbxassetid://4155801252")

--[[
  <string> New image
]]
```

## Destroy UI / Script
```lua
DestroyScript()
```
## Extra

## Update Toggle
```lua
UpdateToggle(Toggle, true)
```

## Update Slider
```lua
UpdateSlider(Slider, 25)

--[[
  Slider
]]
```

## Update DropDown
```lua
UpdateDropdown(Dropdown, {"um", "hello", "redzhub"})

--[[
  {"u ", "hello", "redzhub"}
]]
```
