function SafeZone()
do
    local SZ1 = game:GetService("Workspace"):FindFirstChild("SafeZone")
    if SZ1 then
        SZ1:Destroy()
    end
end

local SafeZone = Instance.new("Part",workspace)
    SafeZone.Name = "SafeZone"
    SafeZone.Anchored = true
    SafeZone.CanCollide = true
    SafeZone.Size = Vector3.new(50,1,50)
end
_G.SafeZone = true
pcall(function()
    SafeZone()
end)
