loadstring(game:HttpGet(("https://raw.githubusercontent.com/REDzHUB/LibraryV2/main/redzLib")))()
MakeWindow({
    Hub = {
      Title = "سكربت العرب / الجزء الثاني",
      Animation = "by : سكربت العرب / الجزء الثاني"
    },
    Key = {
      KeySystem = false,
      Title = "1",
      Description = "",
      KeyLink = "",
      Keys = {"1234"},
      Notifi = {
        Notifications = true,
        CorrectKey = "Running the Script...",
        Incorrectkey = "The key is incorrect",
        CopyKeyLink = "Copied to Clipboard"
      }
    }
  })
  
  --[[
    Hub = {
      Title = "REDz HUB" -- <string> Titulo do seu script
      Animation = "by : redz9999" -- <string> Adiciona um texto na animacão do seu HUB
    },
    Key = {
      KeySystem = <bollean> Adiciona um sistema de chaves
      Title = "Key System" <string> Adiciona um titulo ao seu sistema de chaves
      Description = "" <string> Adiciona uma descrição ao seu sistema de chaves
      KeyLink = "" <string> Adicina o Link onde pega a chave do HUB
      Keys = {"1234"} <table> Adiciona as Chaves
      Notifi = {
        Notifications = true <boolean> Adicina notificações ao sistema de chaves
        CorrectKey = "Running the Script..." <string> notificação quando a chave estiver correta
        Incorrectkey = "The key is incorrect" <string> notificação quando a chave estiver incorreta
        CopyKeyLink = "Copied to Clipboard" <string> notificação quando o link da chave fir copiado
      }
    }
  ]]

  local Main = MakeTab({Name = "السكربتات"})

  --[[
    Name = "Main" <string> Nome da guia
  ]]

  local section = AddSection(Main, {"السكربتات كلها عشوايه"})
  --[[
    {"Teste"} <table> nome da janela
  ]]

  AddButton(Main, {
    Name = "بلوكس فروت",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Domadicoof/Domadicoof/main/Domadichub/NottoGay/Start.ranscript"))()
    end
  })

  AddButton(Main, {
    Name = "بلوكس فروت",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Minhtriettt/Free-Script/main/Chest-Farm.lua"))()
    end
  })

  AddButton(Main, {
    Name = "السكربت  / ريدز بلوكس فروت",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/REDzHUB/BloxFruits/main/redz9999"))()
    end
  })

  AddButton(Main, {
    Name = "سكربت ام ام تو",
    Callback = function()
        loadstring(game:HttpGet(("https://pastebin.com/raw/mT10xnt7"), true))()
    end
  })

  AddButton(Main, {
    Name = "سكربت طيران عربي",
    Callback = function()
        loadstring(game:HttpGet('https://github.com/HUBSXOBOX/HUBSXOBOX/raw/main/Hussin%20Danis'))()
    end
  })

  AddButton(Main, {
    Name = "سكربت بروك هافن نسخ سكنات",
    Callback = function()
        loadstring(game:HttpGet("https://scriptblox.com/raw/Brookhaven-RP-REDz-HUB-6559"))()
    end
  })

  AddButton(Main, {
    Name = "سكربت بروك هافن ادمن الشات",
    Callback = function()
        loadstring(game:HttpGet('https://raw.githubusercontent.com/BloodyBurns/Hex/main/Iv%20Admin%20v3.lua'))()
    end
  })

  AddButton(Main, {
    Name = "سكربت ام ام تو",
    Callback = function()
        loadstring(game:HttpGet("https://scriptblox.com/raw/Murder-Mystery-2-Autofarm-Candy-8839"))()
    end
  })

  AddButton(Main, {
    Name = "سكربت ماب بت سمليتر",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/REDzHUB/PetSimulator99/main/redz9999.lua"))()
    end
  })

  AddButton(Main, {
    Name = "سكربت ماب حرب الوقت حرب السيوف",
    Callback = function()
        loadstring(game:HttpGet('https://raw.githubusercontent.com/anyahubs/swordgame/main/anya.lua'))()
    end
  })

  AddButton(Main, {
    Name = "سكربت ماب بت سمليتر السكربت فيه سكربتات الماب كلها",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/GamerScripter/Game-Hub/main/loader"))()
    end
  })

  AddButton(Main, {
    Name = "سكربت ماب بت سمليتر",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/OfficialPS99Developer/PS99OfficialScript/main/PS99OfficialScript"))()
    end
  })

  AddButton(Main, {
    Name = "X سكربت ماب بت سمليتر من صنعي السكربت",
    Callback = function()
        loadstring(game:HttpGet("https://pastebin.com/raw/kMei7Efr"))()
    end
  })

  AddButton(Main, {
    Name = "سكربت تخريب اقوى من سكربت ايس هوب",
    Callback = function()
        loadstring(game:HttpGet("https://scriptblox.com/raw/Universal-Script-Haxker666-Script-hub-9666"))()
    end
  })

  AddButton(Main, {
    Name = "سكربت يشيل الشات كامل",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/BidoSkinsYT/BidoSkinsYT/main/Fe%20lag%20chat%20Gui"))()
    end
  })

  AddButton(Main, {
    Name = "سكربت ام ام تو عربي",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/VR7ss/VR7/main/MM2"))()
    end
  })

  AddButton(Main, {
    Name = "سكربت اوتو كلك / ريبيث",
    Callback = function()
        -- RX ALMAHRI --
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

  AddButton(Main, {
    Name = "سكربت تخريب الشات",
    Callback = function()
        -- RX ALMAHRI --
    -- ALMAHRI IS HERE --
      _G.Autofarm = true

      while _G.Autofarm == true do

  while wait() do
 
local args = {
         [1] = ".. \226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184"
        .."\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187\226\184\187",
    [2] = "All"
  }

    game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
  wait()
end
end
    end
  })
  
 --[[
    Name = "Botão teste" <string> nome do seu botão
    Callback = function()
      -- funcão do seu botão
    end
  ]]

  local Main = MakeTab({Name = "الاعدادات"})

  --[[
    Name = "Main" <string> Nome da guia
  ]]

  local section = AddSection(Main, {"الاعب"})
  --[[
    {"Teste"} <table> nome da janela
  ]]

  AddColorPicker(Main, {
    Name = "اتخار لون",
    Default = Color3.fromRGB(255, 255, 0),
    Callback = function(Value)
      
    end
  })
  
  --[[
    Name = "Color picker teste" <string> Nome do setor de cores
    Default = Color3.fromRGB(255, 255, 0) <Color3> Define a cor padrão do setor de cores
    Callback = function(Value)
      -- funcão do setor de cores
    end
  ]]

MinimizeButton({
  Image = "1",
  Size = {40, 40},
  Color = Color3.fromRGB(10, 10, 10),
  Corner = true,
  Stroke = false,
  StrokeColor = Color3.fromRGB(255, 0, 0)
})

--[[
  Image = "" <string> imagem do botão
  Size = {40, 40} <table> tamanho do botão
  Color = Color3.fromRGB(10, 10, 10) <Color3>  Cor do fundo do botäo
  Corner = true -- <boolean> Adicina um UICorner
  Stroke = false <boolean> Adiciona um UIStroke
  StrokeColor = Color3.fromRGB(255, 0, 0) <Color3> Cor do UIStroke
]]



  local Main = MakeTab({Name = "التحديثات"})

  --[[
    Name = "Main" <string> Nome da guia
  ]]
  local section = AddSection(Main, {"تحديث رقم 0.1"})
  --[[
    {"Teste"} <table> nome da janela
  ]]

  local Main = MakeTab({Name = "المطورين"})

  --[[
    Name = "Main" <string> Nome da guia
  ]]

  local section = AddSection(Main, {"من قبل / محمد"})
  --[[
    {"Teste"} <table> nome da janela
  ]]

  local section = AddSection(Main, {"مع مساعدة ايوب"})
  --[[
    {"Teste"} <table> nome da janela
  ]]

  local section = AddSection(Main, {"مع مساعدة بلال"})
  --[[
    {"Teste"} <table> nome da janela
  ]]
