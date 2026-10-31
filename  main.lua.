local Players = game:GetService("Players")
local CoreGui = game:GetService("CoreGui")

local gui = Instance.new("ScreenGui")
gui.Name = "DestroyerHub"
gui.ResetOnSpawn = false
gui.Parent = CoreGui

local frame = Instance.new("Frame")
frame.Size = UDim2.new(0, 240, 0, 190)
frame.Position = UDim2.new(0.5, -120, 0.5, -95)
frame.BackgroundColor3 = Color3.fromRGB(20, 20, 25)
frame.Active = true
frame.Draggable = true
frame.Parent = gui

Instance.new("UICorner", frame).CornerRadius =
    UDim.new(0, 10)

local title = Instance.new("TextLabel")
title.Size = UDim2.new(1, 0, 0, 35)
title.BackgroundTransparency = 1
title.Text = "DESTROYER HUB"
title.TextColor3 = Color3.fromRGB(255, 255, 255)
title.TextSize = 18
title.Parent = frame

local toggle = Instance.new("TextButton")
toggle.Size = UDim2.new(0, 200, 0, 35)
toggle.Position = UDim2.new(0, 20, 0, 45)
toggle.Text = "FOV: OFF"
toggle.Parent = frame

local circle = Instance.new("Frame")
circle.Size = UDim2.new(0, 120, 0, 120)
circle.Position = UDim2.new(0.5, -60, 0.5, -60)
circle.BackgroundTransparency = 1
circle.Visible = false
circle.Parent = gui

local stroke = Instance.new("UIStroke")
stroke.Color = Color3.fromRGB(255, 0, 0)
stroke.Thickness = 2
stroke.Parent = circle

Instance.new("UICorner", circle).CornerRadius =
    UDim.new(1, 0)

local active = false

toggle.MouseButton1Click:Connect(function()
    active = not active
    circle.Visible = active
    toggle.Text = active and "FOV: ON" or "FOV: OFF"
end)

local close = Instance.new("TextButton")
close.Size = UDim2.new(0, 200, 0, 30)
close.Position = UDim2.new(0, 20, 0, 90)
close.Text = "FECHAR"
close.Parent = frame

close.MouseButton1Click:Connect(function()
    gui:Destroy()
end)