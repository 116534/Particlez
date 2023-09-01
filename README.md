while true do
----here is the decal particlez
local button = script.Parent
local decal = Instance.new("Decal")
decal.Texture = "rbxassetid://(Decal ID Here)"
local particles = Instance.new("ParticleEmitter") 

particles.Parent = button
particles.Texture = decal.Texture
particles.Rate = 100 

button.MouseButton1Down:Connect(function()
  particles.Enabled = true
end) 

button.MouseButton1Up:Connect(function()
  particles.Enabled = false
end)
