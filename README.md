-- carregar
local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()

local Window = Fluent:CreateWindow({
    Title = "Farm.." .. Fluent.Version,
    TabWidth = 200, Size = UDim2.fromOffset(400, 300), Theme = "Dark"
})

local Tabs = {
    Main = Window:AddTab({ Title = "YT JUBILEU" }),
    Settings = Window:AddTab({ Title = "Settings", Icon = "settings" })
}
-- parágrafos
Tabs.Main:AddParagraph({ Title = "YT JUBILEU", Content = "NADA AKI HEHEHE" })

-- botões
Tabs.Main:AddButton({ Title = "PETS REPETIR..", Callback = function() 
while true do 
local args = {
    [1] = {
        ["ItemType"] = "Pet",
        ["ItemData"] = {
            ["Price"] = -1,
            ["Id"] = 2005,
            ["Name"] = "Moody",
            ["PriceType"] = "SeasonPassPoint"
        }
    }
}

game:GetService("ReplicatedStorage").Remote.SeasonPass.Server.PurchaseMarketItem:InvokeServer(unpack(args))

Wait()
end
end })

-- botões
Tabs.Main:AddButton({ Title = "PETS..", Callback = function() 
local args = {
    [1] = {
        ["ItemType"] = "Pet",
        ["ItemData"] = {
            ["Price"] = -1,
            ["Id"] = 2005,
            ["Name"] = "Moody",
            ["PriceType"] = "SeasonPassPoint"
        }
    }
}

game:GetService("ReplicatedStorage").Remote.SeasonPass.Server.PurchaseMarketItem:InvokeServer(unpack(args))
end })

-- botões
Tabs.Main:AddButton({ Title = "ENERGIA REPETIR..", Callback = function() 
while true do 
local args = {
    [1] = {
        ["ItemType"] = "Energy",
        ["ItemData"] = {
            ["Price"] = -1,
            ["Product"] = 1362659018,
            ["Name"] = "Energy3",
            ["PriceType"] = "SeasonPassPoint"
        }
    }
}

game:GetService("ReplicatedStorage").Remote.SeasonPass.Server.PurchaseMarketItem:InvokeServer(unpack(args))

Wait()
end
end })

-- botões
Tabs.Main:AddButton({ Title = "ENERGIA..", Callback = function() 
local args = {
    [1] = {
        ["ItemType"] = "Energy",
        ["ItemData"] = {
            ["Price"] = -1,
            ["Product"] = 1362659018,
            ["Name"] = "Energy3",
            ["PriceType"] = "SeasonPassPoint"
        }
    }
}

game:GetService("ReplicatedStorage").Remote.SeasonPass.Server.PurchaseMarketItem:InvokeServer(unpack(args))
end })

-- botões
Tabs.Main:AddButton({ Title = "PowerPotion", Callback = function() 
local args = {
    [1] = {
        ["ItemType"] = "Potion",
        ["ItemData"] = {
            ["Price"] = -1,
            ["BoostType"] = "Power",
            ["Name"] = "PowerPotion",
            ["PriceType"] = "SeasonPassPoint"
        }
    }
}

game:GetService("ReplicatedStorage").Remote.SeasonPass.Server.PurchaseMarketItem:InvokeServer(unpack(args))
end })
