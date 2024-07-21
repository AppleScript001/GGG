local Library = loadstring(game:HttpGet("https://pastebin.com/raw/KNBp0LRy"), "Coastified UI")()

local Window = Library:NewWindow("Pet Simulator X", Enum.KeyCode.G)

local Section = Window:NewSection("AutoFarm [Area]")

local Dropdown = Section:CreateDropdown("Select AreaFarm!", {"Town", "Forest", "Beach", "Mine", "Winter", "Glacier", "Desert", "Volcano", "Enchanted Forest", "Ancient Island", "Samurai Island", "Candy Island", "Haunted Island", "Hell Island", "Heaven Island", "Heavens Gate", "Ice Tech", "Tech City", "Dark Tech", "Steampunk", "Steampunk Chest", "Alien Lab", "Alien Forest", "Alien Chest", "Glitch", "Hacker Portal", "Axolotl Ocean", "Axolotl Deep Ocean", "Axolotl Cave", "Pixel Forest", "Pixel Kyoto", "Pixel Alps", "Pixel Vault", "Cat Paradise", "Cat Backyard", "Cat Taiga", "Cat Kingdom", "Cat Throne Room"}, Select, function(Value4)
  PlayerTP = Value4
end)

local Toggle = Section:CreateToggle("Auto Farm", function(Value4)
  _G.AutoFarm = Value4
while _G.AutoFarm do
    
_G.Area = PlayerTP


loadstring(game.HttpGet(game, 'https://raw.githubusercontent.com/zuhnosu/psx-auto-farm/main/main.lua', true))()
wait(0.1)
end
end)

local Toggle = Section:CreateToggle("Auto [Orbs]", function(Value2)
  _G.Orbs = Value2
while _G.Orbs do wait(0.2)
    for i,v in pairs(workspace.__THINGS.Orbs:GetChildren()) do
v.CFrame = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame
end
end
end)
local Toggle = Section:CreateToggle("Auto [Lootbags]", function(Value3)
  _G.Lootbags = Value3
while _G.Lootbags do wait(0.2)
    for i,v in pairs(workspace.__THINGS.Lootbags:GetChildren()) do
v.CFrame = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame
end
end
end)

local Section = Window:NewSection("Diamond Mine")

local Dropdown = Section:CreateDropdown("Select AreaFarm!", {"Paradise Cave", "Cyber Cavern", "Mystic Mine"}, Select, function(Value6)
  PlayerTP = Value6
end)

local Toggle = Section:CreateToggle("Auto Farm", function(Value1)
  _G.AutoFarm = Value1
while _G.AutoFarm do
    
_G.Area = PlayerTP


loadstring(game.HttpGet(game, 'https://raw.githubusercontent.com/zuhnosu/psx-auto-farm/main/main.lua', true))()
wait(0.1)
end
end)

local Toggle = Section:CreateToggle("Auto [Orbs]", function(Value8)
  _G.Orbs1 = Value8
while _G.Orbs1 do wait(0.2)
    for i,v in pairs(workspace.__THINGS.Orbs:GetChildren()) do
v.CFrame = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame
end
end
end)
local Toggle = Section:CreateToggle("Auto [Lootbags]", function(Value7)
  _G.Lootbags1 = Value7
while _G.Lootbags1 do wait(0.2)
    for i,v in pairs(workspace.__THINGS.Lootbags:GetChildren()) do
v.CFrame = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame
end
end
end)

local Section = Window:NewSection("Interactive")

getgenv().Player = game:GetService("Players").LocalPlayer
local Button = Section:CreateButton("Bank", function()
    Player.Character.HumanoidRootPart.CFrame = workspace.__MAP.Interactive.Bank.Pad.CFrame
end)
local Button = Section:CreateButton("Mailbox", function()
    Player.Character.HumanoidRootPart.CFrame = workspace.__MAP.Interactive.Mailbox.Pad.CFrame
end)
local Button = Section:CreateButton("Gold Machine", function()
    Player.Character.HumanoidRootPart.CFrame = workspace.__MAP.Interactive["Gold Machine"].Pad.CFrame
end)
local Button = Section:CreateButton("Pet Collection Machine", function()
    Player.Character.HumanoidRootPart.CFrame = workspace.__MAP.Interactive["Pet Collection Machine"].Pad.CFrame
end)
local Button = Section:CreateButton("Daycare", function()
    Player.Character.HumanoidRootPart.CFrame = workspace.__MAP.Interactive.Daycare.Pad.CFrame
end)
local Button = Section:CreateButton("Upgrade Station", function()
    Player.Character.HumanoidRootPart.CFrame = workspace.__MAP.Interactive["Upgrade Station"].Pad.CFrame
end)
local Button = Section:CreateButton("Fuse Pets", function()
    Player.Character.HumanoidRootPart.CFrame = workspace.__MAP.Interactive["Fuse Pets"].Pad.CFrame
end)
local Button = Section:CreateButton("Rainbow Machine", function()
    Player.Character.HumanoidRootPart.CFrame = workspace.__MAP.Interactive["Rainbow Machine"].Pad.CFrame
end)
local Button = Section:CreateButton("Evolve Machine", function()
    Player.Character.HumanoidRootPart.CFrame = workspace.__MAP.Interactive["Evolve Machine"].Pad.CFrame
end)
local Button = Section:CreateButton("Huge Machine", function()
    Player.Character.HumanoidRootPart.CFrame = workspace.__MAP.Interactive["Huge Machine"].Pad.CFrame
end)

local Section = Window:NewSection("Destroy Gui")

Section:CreateColorPicker("ColorPicker", Color3.fromRGB(235, 64, 52), function(Color)
  print(Color)
end)

Section:CreateButton("Destroy Gui", function()
  Library:Destroy()
end)

repeat wait() until game:IsLoaded()
game:GetService("Players").LocalPlayer.Idled:connect(function()
game:GetService("VirtualUser"):ClickButton2(Vector2.new())
end)
