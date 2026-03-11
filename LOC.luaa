local player = game.Players.LocalPlayer
local RunService = game:GetService("RunService")

local gui = Instance.new("ScreenGui")
gui.Parent = player:WaitForChild("PlayerGui")

local label = Instance.new("TextLabel")
label.Parent = gui
label.Size = UDim2.new(0,300,0,50)
label.Position = UDim2.new(0,10,0,10)
label.TextScaled = true
label.BackgroundTransparency = 0.3
label.Text = "Loading..."

RunService.RenderStepped:Connect(function()
    local char = player.Character
    if char and char:FindFirstChild("HumanoidRootPart") then
        local pos = char.HumanoidRootPart.Position
        label.Text = string.format("X: %.2f  Y: %.2f  Z: %.2f", pos.X, pos.Y, pos.Z)
    end
end)
