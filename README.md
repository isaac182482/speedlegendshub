local a=game.Players.LocalPlayer.PlayerGui
local b=Instance.new("ScreenGui")b.ResetOnSpawn=false b.Parent=a
local c=Instance.new("Frame")c.Size=UDim2.new(0,200,0,250)c.Active=true c.Draggable=true c.BackgroundColor3=Color3.new(0,0,0)c.Parent=b
local d=Instance.new("TextButton")d.Size=UDim2.new(0,150,0,40)d.BackgroundColor3=Color3.new(0,7,0)d.Position=UDim2.new(0,25,0,75)d.Text="Collect-Orb"d.TextScaled=true d.Parent=c
d.MouseButton1Click:Connect(function()
_1=not _1 if _1 then d.BackgroundColor3=Color3.new(1,0,0)else d.BackgroundColor3=Color3.new(0,1,0)end
while _1 do
local _2={"collectOrb","Red Orb","City"}
game:GetService("ReplicatedStorage"):WaitForChild("rEvents"):WaitForChild("orbEvent"):FireServer(unpack(_2))wait(0.2)
end
end)

local e=Instance.new("TextButton")e.Size=UDim2.new(0,150,0,40)e.BackgroundColor3=Color3.new(0,7,0)e.Position=UDim2.new(0,25,0,125)e.Text="Collect-Gems"e.TextScaled=true e.Parent=c
e.MouseButton1Click:Connect(function()
_3=not _3 if _3 then e.BackgroundColor3=Color3.new(1,0,0)else e.BackgroundColor3=Color3.new(0,1,0)end
while _3 do
local _4={"collectOrb","Gem","City"}
game:GetService("ReplicatedStorage"):WaitForChild("rEvents"):WaitForChild("orbEvent"):FireServer(unpack(_4))wait(0.2)
end
end)

local f=Instance.new("TextButton")f.Size=UDim2.new(0,150,0,40)f.BackgroundColor3=Color3.new(0,7,0)f.Position=UDim2.new(0,25,0,175)f.Text="Auto-Rebirth"f.TextScaled=true f.Parent=c
f.MouseButton1Click:Connect(function()
_5=not _5 if _5 then f.BackgroundColor3=Color3.new(1,0,0)else f.BackgroundColor3=Color3.new(0,1,0)end
while _5 do
local _6={"rebirthRequest"}
game:GetService("ReplicatedStorage"):WaitForChild("rEvents"):WaitForChild("rebirthEvent"):FireServer(unpack(_6))wait(0.5)
end
end)

local g=Instance.new("TextButton")g.Size=UDim2.new(0,30,0,30)g.BackgroundColor3=Color3.new(1,0,0)g.Position=UDim2.new(0,10,0,10)g.Text="X"g.TextScaled=true g.Parent=c
g.MouseButton1Click:Connect(function()c.Visible=false end)

local h=Instance.new("TextLabel")h.Name="Credits"h.Size=UDim2.new(0,150,0,30)h.Text="by: zipp.          [beta]"h.Position=UDim2.new(0,25,0,220,0)h.TextColor3=Color3.new(1,1,1)h.TextScaled=false h.BackgroundTransparency=1 h.Parent=c
local i=Instance.new("UIStroke")i.Thickness=1 i.Color=Color3.new(1,1,1)i.Parent=c
local j=Instance.new("UICorner")j.CornerRadius=UDim.new(0,10)j.Parent=c
