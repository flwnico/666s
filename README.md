
local ScreenGui = Instance.new("ScreenGui")
local TextButton = Instance.new("TextButton")



ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

TextButton.Parent = ScreenGui
TextButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextButton.Position = UDim2.new(0, 0, 0.303225815, 0)
TextButton.Size = UDim2.new(0, 200, 0, 50)
TextButton.Font = Enum.Font.SourceSans
TextButton.TextColor3 = Color3.fromRGB(0, 0, 0)
TextButton.TextSize = 14.000



local function INEOD_fake_script() -- TextButton.LocalScript 
	local script = Instance.new('LocalScript', TextButton)

	script.Parent.MouseButton1Click:Connect(function()
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(5.61712837, 3.99802613, -4.92367268, 0.363745719, 9.44902752e-08, -0.931498289, -3.90481247e-08, 1, 8.61909157e-08, 0.931498289, 5.02168618e-09, 0.363745719)
		end)
end
coroutine.wrap(INEOD_fake_script)()
