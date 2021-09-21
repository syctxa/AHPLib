# AHPLib V2
On Delopment
```  
loadstring(game:HttpGet(https://raw.githubusercontent.com/soyandrey/AHPLib/main/AHPLib%20V2))()
```  
**functions**

- Title
- Description
- Label
- Button
- Slider
- Dropdown
- Tabs


**usage**

***
### Example
```lua
--for getting the Lib
local GUI = loadstring(game:HttpGet(https://raw.githubusercontent.com/soyandrey/AHPLib/main/AHPLib%20V2))()
--put the Tile in "Name" and the description in "Description" 
local UI = GUI:CreateWindow("Name","Description")
--put the name of your page in "Page" put the Title of the page in "Page Title" put the page number in "1" like 1 2 3 4, if you want to put the page when you start it "true"
--put the PX you want in thing to thing in "6"
local Page = UI:addPage("Page Title",1,true,6)
--for a label
Page:addLabel("label Text","Label Subtext")
--for a button
Page:addButton("button Text",function(bool)
--put the function you want to execute when it clicked
  print("hello world")
end)
--for a slider
Page:addSlider("Slider Text",16,100,function(value)
--put in "16,100" the slider value. 23,234 or 23,435, put what you want
    print(value)
end)
--for a toogle
Page:addToggle("Toggle Text",function(value)
    print(value)
    if value == false then 
        game.StarterGui:SetCore("SendNotification",{
            Title = "Toggle";
            Text = "false";
        })
    else 
        game.StarterGui:SetCore("SendNotification",{
            Title = "Toggle";
            Text = "true";
        })
    end
end)
--for a textbox
Page:addTextBox("TextBox title","Text",function(value)
    game.StarterGui:SetCore("SendNotification",{
        Title = "Wrote";
        Text = value;
    })
end)
--for dropdown
Page:addDropdown("This is a Dropdown",{"Um","Yep","Lop","GG"},1,function(value)
    game.StarterGui:SetCore("SendNotification",{
        Title = "Selected :";
        Text = value;
    }) 
end)
```


![AHPLIB V2](https://tr.rbxcdn.com/2ad1db09b75954fd8054691ea9e422df/420/420/Decal/Png)

[Get full Documentation](google.com)      

                     _pascalhacks™_                           
