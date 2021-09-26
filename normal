game:GetService("Players").LocalPlayer.Character.Archivable = true
local fakemodel = game:GetService("Players").LocalPlayer.Character:Clone()
fakemodel.Name = "FM"
fakemodel.Parent = game:GetService("Players").LocalPlayer.Character
workspace.Camera.CameraSubject = fakemodel.HumanoidRootPart
game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(0,10500,0) 
for i,v in pairs(game:GetService("Players").LocalPlayer.Character:GetChildren()) do
    if v:IsA("BasePart") then
        v.Anchored = true
end end
game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Anchored = true
game:GetService("Players").LocalPlayer.Character = fakemodel
game:GetService("Players").LocalPlayer.Character.Humanoid.DisplayDistanceType = "None"
workspace.Camera.CameraSubject = fakemodel.Humanoid
game:GetService("Players").LocalPlayer.Character.Humanoid.Died:Connect(function(d)
    workspace[game:GetService("Players").LocalPlayer.Name].Humanoid:TakeDamage(game:GetService("Players").LocalPlayer.Character.Humanoid.Health + 0.01)
 game:GetService("Players").LocalPlayer.Character = workspace[game:GetService("Players").LocalPlayer.Name]
      workspace[game:GetService("Players").LocalPlayer.Name].Humanoid:TakeDamage(game:GetService("Players").LocalPlayer.Character.Humanoid.Health + 0.01)
    end)
