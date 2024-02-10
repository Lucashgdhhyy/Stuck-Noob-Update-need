local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "Stuck Noobs|Blox Fruit [Alpha]", HidePremium = false, SaveConfig = true, ConfigFolder = "OrionTest"})
local Tab = Window:MakeTab({
	Name = "Discord",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

Tab:AddParagraph("Thank you for use Stuck Noob","Please Join On us Discord")
Tab:AddParagraph("Developers","Tubaro Team and LK Team")
Tab:AddParagraph("Beta testers","speedtotimers, lucashelomanu , superscript")
Tab:AddParagraph("A big thank you for","You:D")
OrionLib:MakeNotification({
	Name = "Blox Fruit",
	Content = "Blox Fruit",
	Image = "rbxassetid://4483345998",
	Time = 5
})

local Tab = Window:MakeTab({
	Name = "Farms",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
Tab:AddParagraph("WARING","This hub on alpha its can result on Ban Permanents")
Tab:AddToggle({
	Name = "Auto Farm",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})

Tab:AddDropdown({
	Name = "Mode Farm?",
	Default = "Mele",
	Options = {"Mele", "Sword"},
	Callback = function(Value)
		print(Value)
	end    
})

Tab:AddDropdown({
	Name = "Plataform",
	Default = "Emulator",
	Options = {"Emulator", "Mobile"},
	Callback = function(Value)
		print(Value)
	end    
})

Tab:AddDropdown({
	Name = "Quest?",
	Default = "Yes",
	Options = {"Yes", "No"},
	Callback = function(Value)
		print(Value)
	end    
})

Tab:AddSlider({
	Name = "Click Speed",
	Min = 1000,
	Max = 40000 ,
	Default = 15000,
	Color = Color3.fromRGB(255,255,255),
	Increment = 1,
	ValueName = "Speed",
	Callback = function(Value)
		print(Value)
	end    
})

local Tab = Window:MakeTab({
	Name = "Others Farms",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

Tab:AddToggle({
	Name = "Auto Cdk",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})

Tab:AddToggle({
	Name = "Auto Soul Guitar",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})

Tab:AddToggle({
	Name = "Auto Pirate Raid",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})

local Section = Tab:AddSection({
	Name = "Sea Events"
})

Tab:AddToggle({
	Name = "Auto Sea Best",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})

Tab:AddToggle({
	Name = "Auto Pirate boat",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})

local Section = Tab:AddSection({
	Name = "Sea 2"
})

Tab:AddToggle({
	Name = "Auto ttk",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})

Tab:AddToggle({
	Name = "Auto Factory",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})

Tab:AddToggle({
	Name = "Auto rengoku",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})

Tab:AddToggle({
	Name = "Auto sea 3",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})
local Section = Tab:AddSection({
	Name = "Sea 1"
})

Tab:AddToggle({
	Name = "Auto saber",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})

Tab:AddToggle({
	Name = "Auto sawn sorwd",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})

Tab:AddToggle({
	Name = "Auto sea 2",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})

local Tab = Window:MakeTab({
	Name = "Devil Fruit",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

Tab:AddToggle({
	Name = "Tp For Fruit",
	Default = false,
	Callback = function(Value)
		print("Teleporting")
	end    
})

Tab:AddToggle({
	Name = "Randon Fruit",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})

Tab:AddToggle({
	Name = "Auto Storage",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})


Tab:AddButton({
	Name = "Open Shop",
	Callback = function()
      		print("button pressed")
  	end    
})

Tab:AddButton({
	Name = "Randon Fruit",
	Callback = function()
      		print("button pressed")
  	end    
})

local Tab = Window:MakeTab({
	Name = "Raid",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

Tab:AddToggle({
	Name = "Auto Buy",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})

Tab:AddToggle({
	Name = "Farm Raid",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})

Tab:AddDropdown({
	Name = "select raid",
	Default = "",
	Options = {"flame", "ice", "quake", "dough", "phoenix"},
	Callback = function(Value)
		print(Value)
	end    
})

local Tab = Window:MakeTab({
	Name = "Misc",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
Tab:AddParagraph("Misc","Comming Soon")
local Tab = Window:MakeTab({
	Name = "Config",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
Tab:AddParagraph("Settings","Comming Soon")
local Tab = Window:MakeTab({
	Name = "Fps",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

Tab:AddToggle({
	Name = "Fps Boost",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})
-- Dropdown:Refresh(List<table>,true)
--Dropdown:Set("dropdown option")
OrionLib:Init()
-- destroying the interface: OrionLib:Destroy() 
