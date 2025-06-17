--biblioteca do redz
local redzlib = loadstring(game:HttpGet("https://raw.githubusercontent.com/tbao143/Library-ui/refs/heads/main/Redzhubui"))()

--carregar a window 
local Window = redzlib:MakeWindow({
  Title = "Roblox Realms : Universal ",
  SubTitle = "by roblox realms unv",
  SaveFolder = "realms universal"
})

Window:AddMinimizeButton({
    Button = { Image = "rbxassetid://102060941641123", BackgroundTransparency = 0 },
    Corner = { CornerRadius = UDim.new(35, 1) },
})

local Tab1 = Window:MakeTab({"Discord", "mail"})

Tab1:AddDiscordInvite({
    Name = "Roblox Realms",
    Description = "Join server",
    Logo = "rbxassetid://102060941641123",
    Invite = "https://discord.gg/npb4QZHWSq",
})


local TabScripts = Window:MakeTab({"Scripts", "home"})

local Section = TabMain:AddSection({"BloxFruits"})

--BloxFruits
TabScripts:AddButton({
    Name = "RedzHub",
    Callback = function()
        local Settings = {
    JoinTeam = "Pirates"; -- Pirates / Marines
    Translator = true;   -- true / false
}

loadstring(game:HttpGet("https://raw.githubusercontent.com/tlredz/Scripts/refs/heads/main/main.luau"))(Settings)
    end
})


TabScripts:AddButton({
    Name = "MatsuneHub",
    Callback = function()
        getgenv().Team = "Pirates"
loadstring(game:HttpGet("https://raw.githubusercontent.com/RealMatsune/Rolls-Rocye/refs/heads/main/Loading.lua"))()
    end
})

TabScripts:AddButton({
    Name = "VolcanoHub",
    Callback = function()
        loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/indexeduu/BF-NewVer/refs/heads/main/V3New.lua"))()
    end
})


local Section = TabScripts:AddSection({"Universal"})

-- Universal 
TabScripts:AddButton({
    Name = "Fly",
    Callback = function()
        loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-Gui-Fly-v3-37111"))()
    end
})


TabScripts:AddButton({
    Name = "KzHub",
    Callback = function()
        loadstring(game:HttpGet("https://pastebin.com/raw/sXUtNTkh"))()
    end
})

local TabCreditos = Window:MakeTab({"Creditos", "Info"})

local Paragraph = TabCreditos:AddParagraph({"Developer Hub", "script by Roblox Realms and Team Realms"})

local Paragraph = TabCreditos:AddParagraph({"Status Hub", "script is up to date and working 🟢"})

local Paragraph = TabCreditos:AddParagraph({"join our Discord group to receive updates "})

