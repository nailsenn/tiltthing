local tilt=7
local offset=-90

local rs=game:GetService'RunService'


rs.RenderStepped:Connect(function(dt)
	if pan then
		local y=select(2,cam.CFrame:ToOrientation())
		local shake=math.rad(math.random(-15,15)*math.min(dt,.075))
		local tiltMath=math.cos(y-math.rad(offset))*math.rad(tilt)
		cam.CFrame*=CFrame.fromOrientation(shake,shake,tiltMath)
		--print(math.round(math.deg(y)),tiltMath)
	end
end)
