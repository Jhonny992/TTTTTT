-- carregar
local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()

local Window = Fluent:CreateWindow({
    Title = "Farm.." .. Fluent.Version,
    TabWidth = 200, Size = UDim2.fromOffset(400, 300), Theme = "Dark"
})

local Tabs = {
    Main = Window:AddTab({ Title = "MENU" }),
    Settings = Window:AddTab({ Title = "Settings", Icon = "settings" })
}
-- parágrafos
Tabs.Main:AddParagraph({ Title = "YT JUBILEU", Content = "FARM" })

-- botões
Tabs.Main:AddButton({ Title = "Farm", Callback = function() 
while true do
local args = {
    [1] = workspace.Map.Plots:FindFirstChild("6").Plot.Conveyor.Blocks:FindFirstChild("Better Block")
}

game:GetService("ReplicatedStorage").Network.Build.Buy:FireServer(unpack(args))


local args = {
    [1] = workspace.Map.Plots:FindFirstChild("6").Plot.Conveyor.Blocks:FindFirstChild("Better Air Block")
}

game:GetService("ReplicatedStorage").Network.Build.Buy:FireServer(unpack(args))

local args = {
    [1] = workspace.Map.Plots:FindFirstChild("6").Plot.Conveyor.Blocks:FindFirstChild("Best Block")
}

game:GetService("ReplicatedStorage").Network.Build.Buy:FireServer(unpack(args))

local args = {
    [1] = workspace.Map.Plots:FindFirstChild("6").Plot.Conveyor.Blocks:FindFirstChild("Ultra Motor")
}

game:GetService("ReplicatedStorage").Network.Build.Buy:FireServer(unpack(args))

local args = {
    [1] = workspace.Map.Plots:FindFirstChild("6").Plot.Conveyor.Blocks:FindFirstChild("Good Air Block")
}

game:GetService("ReplicatedStorage").Network.Build.Buy:FireServer(unpack(args))

local args = {
    [1] = workspace.Map.Plots:FindFirstChild("6").Plot.Conveyor.Blocks:FindFirstChild("Ultra Fuel")
}

game:GetService("ReplicatedStorage").Network.Build.Buy:FireServer(unpack(args))

local args = {
    [1] = workspace.Map.Plots:FindFirstChild("6").Plot.Conveyor.Blocks:FindFirstChild("Best Air Block")
}

game:GetService("ReplicatedStorage").Network.Build.Buy:FireServer(unpack(args))
Wait(1)
end
end })

# TTTTTT
