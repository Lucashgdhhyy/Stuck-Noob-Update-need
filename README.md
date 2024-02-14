local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "Stouks X [Pre-Testes]", HidePremium = false, SaveConfig = false, ConfigFolder = "Blade Ball"})
local Tab = Window:MakeTab({
	Name = "Discord",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

OrionLib:MakeNotification({
	Name = "Script Blade Ball",
	Content = "Oi CuzCuz com Ovo:D",
	Image = "rbxassetid://4483345998",
	Time = 5
})

Tab:AddParagraph("Por favor entre no nosso discord","Please Join us discord")	
Tab:AddParagraph("Aviso","Digite o link abaixo no navegador:D para entrar no server")	
Tab:AddButton({
	Name = "https://discord.gg/wn9sxQymcp",
	Callback = function()                       OrionLib:MakeNotification({
		Name = "Error 134",
		Content = "O link nao pode ser copíado digite manualmente",
		Image = "rbxassetid://4483345998",
		Time = 5
	})
      		print("button pressed")
  	end    
})

Tab:AddParagraph("Nao testado em Delta,Trigon Evo,Hydrogen,Vegas X","Testados:Fluxus Arcerus X neon")

local Tab = Window:MakeTab({
	Name = "Combat",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

Tab:AddButton({
	Name = "Auto Parry Hosvile",
	Callback = function()               OrionLib:MakeNotification({
		Name = "Executado",
		Content = "Obrigado por escolher o Stouks X",
		Image = "rbxassetid://4483345998",
		Time = 5
	})
      		print("You are good for select hosvile")                   loadstring(game:HttpGet("https://raw.githubusercontent.com/Hosvile/Refinement/main/MC%3ABlade%20Ball%20Parry",true))()
	end    
})
Tab:AddButton({
	Name = "Auto Parry Red Circle",
	Callback = function()               OrionLib:MakeNotification({
		Name = "Executado",
		Content = "Obrigado por escolher o Stouks X",
		Image = "rbxassetid://4483345998",
		Time = 5
	})                         
      		print("So.....")                    loadstring(game:HttpGet("https://raw.githubusercontent.com/1f0yt/community/main/AutoBlock"))()
	end    
})

Tab:AddButton({
	Name = "Mobile Spam Button",
	Callback = function()               OrionLib:MakeNotification({
		Name = "Executado",
		Content = "Obrigado por escolher o Stouks X",
		Image = "rbxassetid://4483345998",
		Time = 5
	})
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
				game.StarterGui:SetCore("SendNotification", {Title = "Active or Desabilited", Text = "Made By Stouks X", Duration = 1})
			end
			
			button.MouseButton1Click:Connect(function()
				toggle()
				showNotification()
			end)
  	end    
})

Tab:AddDropdown({
	Name = "Curve a bola:Teste",
	Default = "Nenhuma",
	Options = {"Nenhuma", "Frente", "Atras", "Esquerda", "Direita"},
	Callback = function(Value)
		print(Value)
	end    
})

Tab:AddBind({
	Name = "Tecla spamm pc",
	Default = Enum.KeyCode.E,
	Hold = true,
	Callback = function()      
		print("F")
	end    
})


local Tab = Window:MakeTab({
	Name = "Conteudos Premiums",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

Tab:AddParagraph("Aviso","")
Tab:AddParagraph("Essa pagina so ira funcionar se voce tiver a versao premium:D","")
Tab:AddParagraph("So e possivel pegar a versao premium por evento","")


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
