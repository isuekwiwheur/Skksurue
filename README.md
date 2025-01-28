local OrionLib = loadstring(game:https://raw.githubusercontent.com/Xtentacion178/Dgsbab/main/Hrbrr.txt')))()

local Window = OrionLib:MakeWindow({Name = "<font color='rgb(255,0,0)'>Cph3er Hub</font>", HidePremium = false, SaveConfig = true, ConfigFolder = "astralhub"})

--[[
Name = <string> - The name of the UI.
HidePremium = <bool> - Whether or not the user details shows Premium status or not.
SaveConfig = <bool> - Toggles the config saving in the UI.
ConfigFolder = <string> - The name of the folder where the configs are saved.
IntroEnabled = <bool> - Whether or not to show the intro animation.
IntroText = <string> - Text to show in the intro animation.
IntroIcon = <string> - URL to the image you want to use in the intro animation.
Icon = <string> - URL to the image you want displayed on the window.
CloseCallback = <function> - Function to execute when the window is closed.
]]


--[[
Name = <string> - The name of the section.
]]

-- Lista de seleÃ§Ã£o de jogadores para "Goto"
local gotoPlayerList = {}
local selectedGotoPlayer = nil
local avisoToggle = false

local function updatePlayerList()
gotoPlayerList = {}
for _, player in ipairs(game.Players:GetPlayers()) do
table.insert(gotoPlayerList, player.Name)
end
end

updatePlayerList()
