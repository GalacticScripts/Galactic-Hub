local Players = game:GetService("Players")
local RunService = game:GetService("RunService")
local ReplicatedStorage = game:GetService("ReplicatedStorage")
local Library = require(ReplicatedStorage:WaitForChild("Lib"))
local LocalPlayer = Players.LocalPlayer

local function keepSanityFull()
	LocalPlayer:SetAttribute("Sanity", 100)
end
Library.Inject("PlayerLostSanity", keepSanityFull)
LocalPlayer:GetAttributeChangedSignal("Sanity"):Connect(keepSanityFull)
RunService.Heartbeat:Connect(keepSanityFull)
keepSanityFull()
return {}
