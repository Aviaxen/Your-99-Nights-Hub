local Rayfield = loadstring(game:HttpGet("https://sirius.menu/gen2"))()

local window = Rayfield:CreateWindow({ 
    Name = "Your 99 Nights Hub", 
    Subtitle = "By Inky", 
    Theme = "amethyst", 
    Configuration = { 
        AutoSave = true, 
        AutoLoad = true, 
        FileName = "Your 99 Nights Hub" 
    } 
})

local homeTab = window:CreateTab({ Name = "Home", Icon = 93364949241311 })

homeTab:CreateSection({ Name = "Featured" })

homeTab:CreateButton({ Name = "Infinite Yield", Callback = function() 
    loadstring(game:HttpGet("https://raw.githubusercontent.com/edgeiy/infiniteyield/master/source"))() 
end })

homeTab:CreateButton({ Name = "Nameless Admin", Callback = function() 
    loadstring(game:HttpGet("https://raw.githubusercontent.com/ltseverydayyou/Nameless-Admin/main/Source.lua"))() 
end })

homeTab:CreateButton({ Name = "Dex Explorer", Callback = function() 
    loadstring(game:HttpGet("https://github.com/AZYsGithub/DexPlusPlus/releases/latest/download/out.lua"))() 
end })

homeTab:CreateButton({ Name = "Remote Spy", Callback = function() 
    loadstring(game:HttpGet("https://github.com/exxtremestuffs/SimpleSpySource/raw/master/SimpleSpy.lua"))() 
end })

homeTab:CreateSlider({ 
    Name = "Walkspeed", 
    Range = { 20, 150 }, 
    Increment = 1, 
    CurrentValue = 16, 
    Suffix = " studs", 
    Callback = function(Value) 
        local player = game:GetService("Players").LocalPlayer 
        if player and player.Character and player.Character:FindFirstChildOfClass("Humanoid") then 
            player.Character:FindFirstChildOfClass("Humanoid").WalkSpeed = Value 
        end 
    end 
})

local foxnamehubTab = window:CreateTab({ Name = "Foxname Hub", Icon = 93364949241311 })

foxnamehubTab:CreateSection({ Name = "Script" })

foxnamehubTab:CreateButton({ Name = "Foxname Hub", Callback = function() 
    loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-Foxname-65930"))()
end })

local voidwarehubTab = window:CreateTab({ Name = "VoidWare Hub", Icon = 93364949241311 })

voidwarehubTab:CreateSection({ Name = "Script" })

voidwarehubTab:CreateButton({ Name = "VoidWare Hub", Callback = function() 
    loadstring(game:HttpGet("https://files.vapevoidware.xyz/VapeVoidware/VW-Add/main/loader.lua", true))()
end })

local thedarkonehubTab = window:CreateTab({ Name = "The Darkone Hub", Icon = 93364949241311 })

thedarkonehubTab:CreateSection({ Name = "Script" })

thedarkonehubTab:CreateButton({ Name = "The Darkone Hub", Callback = function() 
    loadstring(game:HttpGet('https://raw.githubusercontent.com/TheDarkoneMarcillisePex/Other-Scripts/refs/heads/main/99%20Nights%20In%20The%20Forest%20GUI'))()
end })
