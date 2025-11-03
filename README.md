local Libary = loadstring(game:HttpGet("https://raw.githubusercontent.com/tbao143/Library-ui/refs/heads/main/Redzhubui"))()
workspace.FallenPartsDestroyHeight = -math.huge

local Window = Libary:MakeWindow({
    Title = "Chaos Hub | Brookhaven RP ",
    SubTitle = "by: Luscaa and venom",
    LoadText = "Carregando cafe",
    Flags = "ChaosHub_Broookhaven"
})
Window:AddMinimizeButton({
    Button = { Image = "rbxassetid://131669852271916", BackgroundTransparency = 0 },
    Corner = { CornerRadius = UDim.new(35, 1) },
})

local InfoTab = Window:MakeTab({ Title = "Info", Icon = "rbxassetid://15309138473" })



InfoTab:AddSection({ "Informações do Script" })
InfoTab:AddParagraph({ "Owner / Developer:", "Luscaa and veno." })
InfoTab:AddParagraph({ "Colaborações:", "Blue, sukuna, Magekko, Darkness, Star, Toddy" })
InfoTab:AddParagraph({ "Você está usando:", "Chaos Hub Brookhaven " })
InfoTab:AddParagraph({"Your executor:", executor})

InfoTab:AddSection({ "Rejoin" })
InfoTab:AddButton({
    Name = "Rejoin",
    Callback = function()
        local TeleportService = game:GetService("TeleportService")
        TeleportService:TeleportToPlaceInstance(game.PlaceId, game.JobId, game.Players.LocalPlayer)
    end
})



local TrollTab = Window:MakeTab({ Title = "Scripts Trolls", Icon = "rbxassetid://13364900349" })

