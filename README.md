local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "Stouks X [Beta V1.1]", HidePremium = false, SaveConfig = false, ConfigFolder = "Blade Ball"})
local Tab = Window:MakeTab({
	Name = "Combat",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

OrionLib:MakeNotification({
	Name = "Script Blade Ball",
	Content = "Please Buy the premium edition",
	Image = "rbxassetid://4483345998",
	Time = 5
})

Tab:AddButton({
	Name = "Auto Parry Hosvile",
	Callback = function()
      		print("You are good for select hosvile")                   loadstring(game:HttpGet("https://raw.githubusercontent.com/Hosvile/Refinement/main/MC%3ABlade%20Ball%20Parry",true))()
	end    
})
Tab:AddButton({
	Name = "Auto Parry Red Circle",
	Callback = function()
      		print("So.....")                    loadstring(game:HttpGet("https://raw.githubusercontent.com/1f0yt/community/main/AutoBlock"))()
	end    
})

Tab:AddButton({
	Name = "Mobile Spam Buttion",
	Callback = function()
      		print("Uhhhhhhh i need remove the giant code of script")                        --[[
				WARNING: Heads up! This script has not been verified by ScriptBlox. Use at your own risk!
			]]
			local gui, frame, button = Instance.new("ScreenGui", game.CoreGui), Instance.new("Frame"), Instance.new("TextButton")
			gui.ResetOnSpawn = false
			frame.Size, frame.Position, frame.BackgroundColor3, frame.BorderSizePixel, frame.Active, frame.Draggable, frame.Parent = UDim2.new(0, 150, 0, 75), UDim2.new(0, 10, 0, 10), Color3.new(0, 0, 0), 0, true, true, gui
			button.Text, button.Size, button.Position, button.BackgroundColor3, button.BorderColor3, button.BorderSizePixel, button.Font, button.TextColor3, button.TextSize, button.Parent = "Stouks X", UDim2.new(1, -20, 1, -20), UDim2.new(0, 10, 0, 10), Color3.new(0, 0, 0), Color3.new(), 2, Enum.Font.SourceSans, Color3.new(1, 1, 1), 16, frame
			
			local activated = false
			
			local function toggle()
				activated, button.Text = not activated, activated and "Desabilited" or "Actived"
				
				while activated do
					local args = {1.5, CFrame.new(-254.29, 112.14, -119.27) * CFrame.Angles(-2.03, 0.57, 2.31), {["2617721424"] = Vector3.new(-273.40, -724.80, -20.92)}, {910, 154}}
					game:GetService("ReplicatedStorage").Remotes.ParryAttempt:FireServer(unpack(args))
					game:GetService("RunService").Heartbeat:Wait()
					button.BorderColor3 = Color3.new(math.random(), math.random(), math.random())
				end
			end
			
			local function showNotification()
				game.StarterGui:SetCore("SendNotification", {Title = "Active or Desabilitef", Text = "Made By Stouks X", Duration = 0})
			end
			
			button.MouseButton1Click:Connect(function()
				toggle()
				showNotification()
			end)
  	end    
})

--[[
Name = <string> - The name of the textbox.
Default = <string> - The default value of the textbox.
TextDisappear = <bool> - Makes the text disappear in the textbox after losing focus.
Callback = <function> - The function of the textbox.
]]

-- Dropdown:Refresh(List<table>,true)
--Dropdown:Set("dropdown option")
OrionLib:Init()
-- destroying the interface: OrionLib:Destroy()
