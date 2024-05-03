-- RX ALMAHRI --
OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "سكربت عربي", HidePremium = false, SaveConfig = true, ConfigFolder = "OrionTest"})

--[[
Name = <string> - The name of the UI.
HidePremium = <bool> - Whether or not the user details shows Premium status or not.
SaveConfig = <bool> - Toggles the config saving in the UI.
ConfigFolder = <string> - The name of the folder where the configs are saved.
IntroEnabled = <bool> - Whether or not to show the intro animation.
IntroText = <BloodTheme> - Text to show in the intro animation.
IntroIcon = <BloodTheme> - URL to the image you want to use in the intro animation.
Icon = <string> - URL to the image you want displayed on the window.
CloseCallback = <function> - Function to execute when the window is closed.
]]local Tab = Window:MakeTab({
	Name = "👑🔥التنقل للتدريب🔥👑",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
 
--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "👑🔥سكربتنا فقط لل لماب  لا اكثر ولا غير🔥👑"
})

--[[
Name = <BloodTheme> - The name of the section.
  ]]Tab:AddButton({
	Name = "👑🔥 اتنقل الى التدريب",
	Callback = function()
      		print("button pressed")
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1100, 50, -2800)
                    end    
              })
              
              Tab:AddButton({
                  Name = "👑🔥 2 تدريب",
                  Callback = function()
                            print("button pressed")
              
              game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-500, 300, -2000)
              wait(0.5)
              game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-500, 50, -6000)
              wait(0.5)
              game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1000, 50, -3004)
              wait(0.9)
              game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1000, 50, -3004)
  	end    
})

 
--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "👑🔥سكربت اوتو كلك🔥👑"
})
 
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "👑🔥 سكربت اوتو كلك",
	Callback = function()
      		print("button pressed")-- RX ALMAHRI --
              _G.AutoClick = true
              spawn(function()
              while _G.AutoClick == true do
              local args = {
                  [1] = 1
              }
 
 
                    game:GetService("ReplicatedStorage").Aero.AeroRemoteServices.ClickService.Click:FireServer(unpack(args))
                 wait()
                end
              end)
 
              spawn(function()
              _G.AutoRebirth = true
              while _G.AutoRebirth == true do
              local args = {
                  [1] = 100
              }
 
                    game:GetService("ReplicatedStorage").Aero.AeroRemoteServices.RebirthService.BuyRebirths:FireServer(unpack(args))
                  wait()
                end
              end)
  	end    
})
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "✋🛑 ايقاف اوتو كلك",
	Callback = function()
      		print("button pressed")-- RX ALMAHRI --
              _G.AutoClick = false
              spawn(function()
              while _G.AutoClick == false do
              local args = {
                  [1] = 1
              }
 
 
                    game:GetService("ReplicatedStorage").Aero.AeroRemoteServices.ClickService.Click:FireServer(unpack(args))
                 wait()
                end
              end)
 
              spawn(function()
              _G.AutoRebirth = false
              while _G.AutoRebirth == false do
              local args = {
                  [1] = 100
              }
 
                    game:GetService("ReplicatedStorage").Aero.AeroRemoteServices.RebirthService.BuyRebirths:FireServer(unpack(args))
                  wait()
                end
              end)
  	end    
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "👑🔥سكربت قتل الكل🔥👑"
})

--[[
Name = <BloodTheme> - The name of the section.
  ]]Tab:AddButton({
    Name = "👑🔥 سكربت قتل الكل",
    Callback = function()
            print("button pressed")
            for i,v in pairs (game:GetService("Players"):GetPlayers()) do
              pcall(function()
             local A_1 = v.Character.Humanoid
             local A_2 = 0
             local Event = game:GetService("Players").LocalPlayer.Character.HitEvent
             Event:FireServer(A_1, A_2)
             end)
             end
      end    
  })


--[[
Name = <string> - The name of the UI.
HidePremium = <bool> - Whether or not the user details shows Premium status or not.
SaveConfig = <bool> - Toggles the config saving in the UI.
ConfigFolder = <string> - The name of the folder where the configs are saved.
IntroEnabled = <bool> - Whether or not to show the intro animation.
IntroText = <BloodTheme> - Text to show in the intro animation.
IntroIcon = <BloodTheme> - URL to the image you want to use in the intro animation.
Icon = <string> - URL to the image you want displayed on the window.
CloseCallback = <function> - Function to execute when the window is closed.
]]local Tab = Window:MakeTab({
	Name = "👑🔥سكربتات",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
 
--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "👑🔥 سكربتات"
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "🍇سكربتات بلوكس فروت🍇"
})

--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "🍇(1) سكربت بلوكس فروت🍇",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/Domadicoof/Domadicoof/main/Domadichub/NottoGay/Start.ranscript"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🍇(2) سكربت بلوكس فروت🍇",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://raw.githubusercontent.com/AXCScript/KayMobile/main/Script-Loader'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🍇(3) سكربت بلوكس فروت🍇",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/Minhtriettt/Free-Script/main/MTriet-Hub.lua"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🍇(4) سكربت بلوكس فروت🍇",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/xQuartyx/DonateMe/main/OldBf"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🍇(5) سكربت بلوكس فروت🍇",
	Callback = function()
      		print("button pressed") loadstring(game:HttpGet("https://raw.githubusercontent.com/NickelHUBB/SonicTuru/main/Protected-25.lua"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🍇(6) سكربت بلوكس فروت🍇",
	Callback = function()
      		print("button pressed")_G.HohoVersion = "v3" 

loadstring(game:HttpGet('https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🍇(7) سكربت بلوكس فروت🍇",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/ThunderZ-05/HUB/main/Main/Chest/AllDevice.lua"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🍇(8) سكربت بلوكس فروت🍇",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/xQuartyx/DonateMe/main/OldBf"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🍇(9) سكربت بلوكس فروت🍇",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/Minhtriettt/Free-Script/main/Chest-Farm.lua"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🍇(10) سكربت بلوكس فروت🍇",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI'))()
  	end    
})
--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🍇(11) سكربت بلوكس فروت🍇",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/REDzHUB/BloxFruits/main/redz9999"))()
  	end    
})


--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "⚔️MM2سكربتات⚔️"
})

--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "⚔️(1) MM2سكربت⚔️",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/CriShoux/OwlHub/master/OwlHub.txt"))();
-- Like and SUBBBBB
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "⚔️(2) MM2سكربت⚔️",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/Ethanoj1/EclipseMM2/master/Script", true))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "⚔️(3) MM2سكربت⚔️",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://pastebin.com/raw/1shHyM48"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "⚔️(4) MM2سكربت⚔️",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/Ethanoj1/EclipseMM2/master/Script", true))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "⚔️(5) MM2سكربت⚔️",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/DreadzHub2/DreadzHub-Scripts-FR/main/Loader"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "⚔️(6) MM2سكربت⚔️",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/Drifter0507/GUIS/main/MURDER%20MYSTERY%202", true))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "⚔️(7) MM2سكربت⚔️",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet(('https://raw.githubusercontent.com/MarsQQ/ScriptHubScripts/master/MM2%20Admin%20Panel'),true))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "⚔️(8) MM2سكربت⚔️",
	Callback = function()
      		print("button pressed")loadstring(game:GetObjects("rbxassetid://4001118261")[1].Source)()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "⚔️(9) MM2سكربت⚔️",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet(("https://pastebin.com/raw/mT10xnt7"), true))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "⚔️(10) MM2سكربت⚔️",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://scriptblox.com/raw/Murder-Mystery-2-Autofarm-Candy-8839"))()
  	end    
})


--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "🏠Brookhavenسكربتات🏠"
})

--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "🏠سكربت بروك هافن ادمن شات🏠",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://raw.githubusercontent.com/BloodyBurns/Hex/main/Iv%20Admin%20v3.lua'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🏠سكربت بروك هافن ايس هوب🏠",
	Callback = function()
      		print("button pressed")loadstring (game: HttpGet ("https://raw.githubusercontent.com/IceMael7/NewIceHub/main/Brookhaven")) ()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🏠سكربت بروك هافن قتل🏠",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/zetkan/zetkan/main/zetkans"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🏠سكربت تخريب بروك هافن🏠",
	Callback = function()
      		print("button pressed")loadstring("\108\111\97\100\115\116\114\105\110\103\40\103\97\109\101\58\72\116\116\112\71\101\116\40\34\104\116\116\112\115\58\47\47\114\97\119\46\103\105\116\104\117\98\117\115\101\114\99\111\110\116\101\110\116\46\99\111\109\47\65\99\117\114\97\88\48\52\57\47\111\98\102\117\115\99\97\116\101\100\83\99\114\105\112\116\115\47\109\97\105\110\47\75\105\108\108\71\117\105\34\41\41\40\41\10")()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🏠(2) سكربت تخريب في بروك هافن🏠",
	Callback = function()
      		print("button pressed")loadstring("\108\111\97\100\115\116\114\105\110\103\40\103\97\109\101\58\72\116\116\112\71\101\116\40\34\104\116\116\112\115\58\47\47\114\97\119\46\103\105\116\104\117\98\117\115\101\114\99\111\110\116\101\110\116\46\99\111\109\47\65\99\117\114\97\88\48\52\57\47\111\98\102\117\115\99\97\116\101\100\83\99\114\105\112\116\115\47\109\97\105\110\47\75\105\108\108\71\117\105\34\41\41\40\41\10")()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]
Tab:AddButton({
	Name = "🏠(1) سكربت بروك هافن ادمن🏠",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🏠(2) سكربت بروك هافن ادمن🏠",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/FilteringEnabled/NamelessAdmin/main/Source"))();
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🏠(3) سكربت بروك هافن ادمن🏠",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🏠سكربت بروك هافن نسخ اسكنات🏠",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://scriptblox.com/raw/Brookhaven-RP-REDz-HUB-6559"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🏠سكربت بروك هافن نجمه🏠",
	Callback = function()
      		print("button pressed")loadstring (game: HttpGet ("https://raw.githubusercontent.com/IceMael7/AvatarUnlocker/main/IceHub")) ()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🏠سكربت بروك هافن طيران سيارة 🏠",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://pastebin.com/raw/MHE1cbWF"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🏠سكربت بروك هافن مشيات🏠",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/GamingScripter/Animation-Hub/main/Animation%20Gui", true))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🏠سكربت بروك هافن كور بروكس🏠",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://pastebin.com/raw/H5yx10Jq'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🏠سكربت بروك هافن كيبورد🏠",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://pastebin.com/raw/eCpipCTH"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🏠سكربت ماب بيوت العرب ادمن🏠",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/xWANTED333/scripts/main/MapAlBiot.Lua"))()
  	end    
})


--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "💪Muscle Legends سكربتات"
})
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "💪(1) Muscle Legends سكربت",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/ahmadsgamer2/Speed-Hub-X/main/SpeedHubX"))()
  	end    
})
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "💪(2) Muscle Legends سكربت",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/Nadir3709/ScriptHub/main/KeySystem"))()
  	end    
})
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "💪(3) Muscle Legends سكربت",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/harisiskandar178/Roblox-Script/main/Muscle%20Legend"))()
  	end    
})


--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "👑🔥سكربتات كل المابات 🔥👑"
})

--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "👑🔥سكربت طيران عربي🔥👑",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://github.com/HUBSXOBOX/HUBSXOBOX/raw/main/Hussin%20Danis'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "👑🔥سكربت سرعه عربي 🔥👑",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://pastebin.com/raw/0m52kRnj"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "👑🔥سكربت الاختفاء🔥👑",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://pastebin.com/raw/AYtzGEPb'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "👑🔥سكربت مراقبه الناس🔥👑",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://pastebin.com/raw/wyvdb7gr'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "👑🔥سكربت تلبورت🔥👑",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet(("https://pastebin.com/raw/YNVbeqPy")))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "👑🔥سكربت سبام🔥👑",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://scriptblox.com/raw/Universal-Script-Fe-Message-Spammer-4637"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "👑🔥سكربت المشي علي الهواء🔥👑",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/Float'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "👑🔥HDRسكربت جودا🔥👑",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/TPC12/RTX-Script-wow/main/RTX%20Script%20Roblox"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "👑🔥ESPسكربت🔥👑",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://scriptblox.com/raw/Universal-Script-Fates-ESP-4437"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "👑🔥سكربت اختراق جدران👑🔥",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://pastebin.com/raw/B5xRxTnk",true))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "👑🔥سكربت تيليسكوب👑🔥",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://pastebin.com/raw/8T0STS4f'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "👑🔥سكربت الشقلبة🔥👑",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://pastebin.com/raw/yjxXnxbS'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "👑🔥سكربت سبايدر مان🔥👑",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet(('https://pastebin.com/raw/2X0hKUgq'),true))()
  	end    
})


--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "⛹️‍♂️BladeBallسكربتات⛹️‍♂️"
})

--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "⛹️‍♂️(1) BladeBallسكربت⛹️‍♂️",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/3345-c-a-t-s-u-s/-beta-/main/AutoParry.lua"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "⛹️‍♂️(2) BladeBallسكربت⛹️‍♂️",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://scriptblox.com/raw/Blade-Ball-Valkyrie-Hub-Rage-8974"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "⛹️‍♂️(3) BladeBallسكربت⛹️‍♂️",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet(('https://pastebin.com/raw/Hqr4NnFU'),true))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "⛹️‍♂️(4) BladeBallسكربت⛹️‍♂️",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/1f0yt/community/main/AutoBlock"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "⛹️‍♂️(5) BladeBallسكربت⛹️‍♂️",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://scriptblox.com/raw/Blade-Ball-Valkryie-Hub-Mobile-Script-8946"))()
  	end    
})


--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "⚔️ سكربتات ماب حرب السيوف اسرق الوقت من عدوك"
})

--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "⚔️(1) سكربت ماب حرب السيوف",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://raw.githubusercontent.com/anyahubs/swordgame/main/anya.lua'))()
  	end    
})


--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "🐶🐱X سكربتات ماب بت سمليتر 99 و🐱🐶"
})

--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "🐶🐱(1) سكربت ماب بت سمليتر🐱🐶",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/REDzHUB/PetSimulator99/main/redz9999.lua"))()
  	end    
})
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "🐶🐱(2) سكربت ماب بت سمليتر السكربت فيه سكربتات الماب كلها🐱🐶",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/GamerScripter/Game-Hub/main/loader"))()
  	end    
})
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "🐶🐱(3) سكربت ماب بت سمليتر🐱🐶",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/OfficialPS99Developer/PS99OfficialScript/main/PS99OfficialScript"))()
  	end    
})
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "🐶🐱(4) X سكربت ماب بت سمليتر من صنعي السكربت🐱🐶",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://pastebin.com/raw/kMei7Efr"))()
  	end    
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "👻Doorsسكربتات👻"
})

--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "👻(1) Doorsسكربت👻",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet(('https://pastebin.com/raw/R8QMbhzv')))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "👻(2) Doorsسكربت👻",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/MrNeRD0/Doors-Hack/main/NeRDV5.lua"))()
  	end    
})


--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "🔨Flee the Facilityسكربتات🔨"
})

--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "🔨(1) Flee the Facilityسكربت🔨",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://raw.githubusercontent.com/Aboahaogsigsigaivva/__Scripts/__Main/__Code/__FleeTheFacility.lua'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🔨(2) Flee the Facilityسكربت🔨",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/Drifty96/ftfgui/main/ftfgui", true))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🔨(3) Flee the Facilityسكربت🔨",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://scriptblox.com/raw/Universal-Script-NexusHub-8624"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🔨(4) Flee the Facilityسكربت🔨",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://scriptblox.com/raw/Flee-the-Facility-Semi-Universal-7452"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🔨(5) Flee the Facilityسكربت🔨",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://scriptblox.com/raw/Universal-Script-Space-Hub-7295"))()
  	end    
})


--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "🔫Breaking Point سكربتات🔫"
})

--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "🔫 (1) Breaking Pointسكربت🔫",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/H4R7NHacks/Obfuscated/master/Breaking%20Point%20H4R7N%20Hack.lua"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]Tab:AddButton({
	Name = "🔫 (2) Breaking Pointسكربت🔫",
	Callback = function()
      		print("button pressed")--Sub to Squidfan420
loadstring(game:HttpGet("https://raw.githubusercontent.com/ColdStep2/Breaking-Point-Funny-Squid-Hax/main/Breaking%20Point%20Funny%20Squid%20Hax",true))();
  	end    
})


--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "⚽TPSسكربتات⚽"
})

--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "⚽(1) TPSسكربت⚽",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://raw.githubusercontent.com/hussain1323232234/My-Scripts/main/Street%20Soccer'))()
  	end    
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "😏🔥 سكربتات من صنعي القديمه"
})
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "😏🔥(1) سكربت من صنع ولد خالي",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://pastebin.com/raw/1mnk5u77"))()
  	end    
})
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "😏🔥(2) سكربت البداية انا و ولد خالي",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://pastebin.com/raw/6bYnWn2j"))()
  	end    
})
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "😏🔥(3) سكربت تسليك",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://pastebin.com/raw/wNNrAbFE"))()
  	end    
})
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "😏🔥(4) سكربت من صنعي",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://pastebin.com/raw/XFP6SsHD"))()
  	end    
})
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "😏🔥(5) سكربت من صنعي",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://pastebin.com/raw/QqSKzTJW"))()
  	end    
})
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "😏🔥(6) سكربت من صنعي",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://pastebin.com/raw/rEr0Rjfj"))()
  	end    
})
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "😏🔥(7) سكربت من صنعي",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://pastebin.com/raw/DkTTgPtA"))()
  	end    
})


--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]

--[[
Title = <string> - The title of the notification.
Content = <string> - The content of the notification.
Image = <string> - The icon of the notification.
Time = <number> - The duration of the notfication.
]]local Section = Tab:AddSection({
	Name = "🔥 افضل سكربتات في سكربت احلام العصر"
})
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "🔥(1) سكربت عربي هو سكربت انيا احلام العصر",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://raw.githubusercontent.com/anyahubs/Hub/main/anyahubV1.lua'))()
  	end    
})
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "🔥(2) سكربت انجليزي هو سكربت لاق احلام العصر",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://gist.githubusercontent.com/H20CalibreYT/462f6e6236a9371130f113def6549bb1/raw/'))()
  	end    
})
--[[
Title = <string> - The title of the notification.
Content = <string> - The content of the notification.
Image = <string> - The icon of the notification.
Time = <number> - The duration of the notfication.
]]local Section = Tab:AddSection({
	Name = "🙃👍 لا حد يسالني ليش السكربت حقي اسمه كذا"
})
--[[
Title = <string> - The title of the notification.
Content = <string> - The content of the notification.
Image = <string> - The icon of the notification.
Time = <number> - The duration of the notfication.
]]local Section = Tab:AddSection({
	Name = "🔥 افضل سكربت لتسوي سكربت اوتو كلك او اي سكربت تبيه"
})
--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "🔥(1) سكربت كودي ذا السكربت / احلام العصر",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://github.com/exxtremestuffs/SimpleSpySource/raw/master/SimpleSpy.lua"))()
  	end    
})


--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]

--[[
Title = <string> - The title of the notification.
Content = <string> - The content of the notification.
Image = <string> - The icon of the notification.
Time = <number> - The duration of the notfication.
]]local Section = Tab:AddSection({
	Name = "🐷piggyسكربتات ماب🐷"
})

--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "🐷piggyسكربت ماب🐷",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://scriptblox.com/raw/Universal-Script-T-HUB-7384"))()
  	end    
})


--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "⚠️سكربتات هاكات روبلوكس⚠️"
})

--[[
Name = <string> - The name of the section.
]]Tab:AddButton({
	Name = "⚠️Arceus X سكربت هاك⚠️",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/AZYsGithub/chillz-workshop/main/Arceus%20X%20V3"))()
  	end    
})


--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]
local Tab = Window:MakeTab({
	Name = "🔧الاعدادات🔧",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "🔧الاعدادات🔧"
})

Tab:AddColorpicker({
	Name = "🟥⬜⬛اختار لون السكربت 🟥⬜⬛",
	Default = Color3.fromRGB(255, 0, 0),
	Callback = function(Value)
		print(Value)
	end	  
})

--[[
Name = <string> - The name of the colorpicker.
Default = <color3> - The default value of the colorpicker.
Callback = <function> - The function of the colorpicker.
]]local Tab = Window:MakeTab({
	Name = "🛠التحديثات🛠",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "🛠بضيف سكربتات اكتر قريبا🛠"
})

--[[
Name = <string> - The name of the section.
]]local Section = Tab:AddSection({
	Name = "🛠تحديث رقم0.1🛠"
})

--[[
Name = <string> - The name of the section.
]]OrionLib:MakeNotification({
	Name = "👑🔥لاتفعيل الاسكربت 🔥👑",
	Content = "👑🔥شكرا لك لاتفعيل الاسكربت🔥👑",
	Image = "rbxassetid://4483345998",
	Time = 10
})

--[[
Title = <string> - The title of the notification.
Content = <string> - The content of the notification.
Image = <string> - The icon of the notification.
Time = <number> - The duration of the notfication.
]]
