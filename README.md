loadstring(game:HttpGet(("https://raw.githubusercontent.com/ahmidd409/TrollX-V2/refs/heads/main/Red")))()
MakeWindow({
  Hub = {
    Title = "EZ_HUB |1.0V|BROOKHAVEN ",
    Animation = "جار تحميل..."
  },
  Key = {
    KeySystem = true,
    Title = "Key System",
    Description = "انضم قناتي لل حصول عل مفتاح",
    KeyLink = "https://t.me/EZ_HUB1",
    Keys = {"abb55"},
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
Main = MakeTab({Name = "معلومات"})
local Image = AddImageLabel(Main, {
  Name = "قنات سكربت ",
  Image = "rbxassetid://136300057076089"
})
AddButton(Main, {
  Name = "نسخ حسابي روبلوكس",
  Callback = function()
    setclipboard('VR_2MS')
  end
})
AddButton(Main, {
  Name = "نسخ حسابي تيك توك",
  Callback = function()
    setclipboard('it_gk9')
  end
})
local Paragraph = AddParagraph(Main, {"السيرفر "})
-- Create a label to show the number of players
local playerCountLabel = AddTextLabel(Main, "الاعبين في السيرفر: " .. #game.Players:GetPlayers())

-- Função para atualizar o número de jogadores quando alguém entra ou sai
local function updatePlayerCount()
    playerCountLabel.Text = "الاعبين في السيرفر: " .. #game.Players:GetPlayers()
end

-- Conecta a função ao evento de entrada de novos jogadores
game.Players.PlayerAdded:Connect(updatePlayerCount)

-- Conecta a função ao evento de saída de jogadores
game.Players.PlayerRemoving:Connect(updatePlayerCount)

-- Atualiza a contagem de jogadores no início (caso tenha jogadores ao carregar o script)
updatePlayerCount()

-- Criando a TextLabel
local Label = AddTextLabel(Main, "")

-- Função para atualizar o tempo na TextLabel
local function updateTime(label)
    while true do
        local currentTime = os.date("%H:%M:%S")
        label.Text = "وقت: " .. currentTime
        wait(1)  -- Atualiza a cada segundo
    end
end

-- Iniciando a atualização da TextLabel
coroutine.wrap(updateTime)(Label)
local Main = MakeTab({Name = "تحديثات القادمه"})

--[[
  Name = "Main" <string> Nome da guia
]]
local Paragraph = AddParagraph(Main, {"الإضافات القادمه"})
local section = AddSection(Main, {"اضافه اكسوورات أكثر "})
local section = AddSection(Main, {"اضافه أجسام وارحل أكثر "})
local section = AddSection(Main, {"اضافه أشياء اخراء"})
local Main = MakeTab({Name = "الرؤوس والرجل"})

--[[
  Name = "Main" <string> Nome da guia
]]
AddButton(Main, {
  Name = "رجل مقطوعه ",
  Callback = function()
    local args = {
    [1] = "CharacterChange",
    [2] = {
        [1] = 1,
        [2] = 1,
        [3] = 1,
        [4] = 139607718,
        [5] = 1,
        [6] = 1
    },
    [3] = "Roblox20"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))
  end
})

AddButton(Main, {
  Name = "رجل مقطوعه 2",
  Callback = function()
    local args = {
    [1] = "CharacterChange",
    [2] = {
        [1] = 1,
        [2] = 1,
        [3] = 1,
        [4] = 1,
        [5] = 139607673,
        [6] = 1
    },
    [3] = "Roblox20"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "راس مخفي",
  Callback = function()
    local args = {
    [1] = "CharacterChange",
    [2] = {
        [1] = 1,
        [2] = 1,
        [3] = 1,
        [4] = 1,
        [5] = 1,
        [6] = 134082579
    },
    [3] = "Roblox20"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))
wait(0.1)
  end
})

AddButton(Main, {
  Name = "راس روبوت",
  Callback = function()
    local args = {
    [1] = "CharacterChange",
    [2] = {
        [1] = 1,
        [2] = 1,
        [3] = 1,
        [4] = 1,
        [5] = 1,
        [6] = 3210773801
    },
    [3] = "Roblox20"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))
wait(0.1)
  end
})

AddButton(Main, {
  Name = "راس روكر",
  Callback = function()
    local args = {
    [1] = "CharacterChange",
    [2] = {
        [1] = 1,
        [2] = 1,
        [3] = 1,
        [4] = 1,
        [5] = 1,
        [6] = 16580493236
    },
    [3] = "Roblox20"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))
wait(0.1)
  end
})
AddButton(Main, {
  Name = "رجل العظام الرصاصي",
  Callback = function()
    print("Clicked")local args = {
    [1] = "CharacterChange",
    [2] = {
        [1] = 1,
        [2] = 1,
        [3] = 1,
        [4] = 17500249989,
        [5] = 1,
        [6] = 1
    },
    [3] = "Roblox20"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "رجل العظام السود",
  Callback = function()
    print("Clicked")local args = {
    [1] = "CharacterChange",
    [2] = {
        [1] = 1,
        [2] = 1,
        [3] = 1,
        [4] = 14547162578,
        [5] = 1,
        [6] = 1
    },
    [3] = "Roblox20"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "رجل رول",
  Callback = function()
    print("Clicked")local args = {
    [1] = "CharacterChange",
    [2] = {
        [1] = 1,
        [2] = 1,
        [3] = 1,
        [4] = 3230472745,
        [5] = 1,
        [6] = 1
    },
    [3] = "Roblox20"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))
  end
})
local Main = MakeTab({Name = "اجسام"})

--[[
  Name = "Main" <string> Nome da guia
]]
AddButton(Main, {
  Name = "جسم ايمو",
  Callback = function()
print("Clicked")local args = {
[1] = "CharacterChange",
[2] = {
[1] = 96491916349570,
[2] = 76683091425509,
[3] = 75159926897589,
[4] = 1,
[5] = 1,
[6] = 1
},
[3] = "YinHub"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))

  
  end
})
AddButton(Main, {
  Name = "بنية جسم",
  Callback = function()
print("Clicked")local args = {
[1] = "CharacterChange",
[2] = {
[1] = 96491916349570,
[2] = 14854350570,
[3] = 14854350451,
[4] = 1,
[5] = 1,
[6] = 1
},
[3] = "YinHub"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))

  end
})
AddButton(Main, {
  Name = "ايد القزومة",
  Callback = function()
print("Clicked")local args = {
[1] = "CharacterChange",
[2] = {
[1] = 16214246112,
[2] = 16214249513,
[3] = 16214251181,
[4] = 1,
[5] = 1,
[6] = 1
},
[3] = "YinHub"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))

  end
})
AddButton(Main, {
  Name = "كوبي جسم",
  Callback = function()
print("Clicked")local args = {
[1] = "CharacterChange",
[2] = {
[1] = 86499666,
[2] = 27112039,
[3] = 27112052,
[4] = 27112068,
[5] = 27112056,
[6] = 1
},
[3] = "YinHub"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))

  end
})


AddButton(Main, {
  Name = "رول قادح 🤯",
  Callback = function()
print("Clicked")local args = {
[1] = "CharacterChange",
[2] = {
[1] = 27112025,
[2] = 27112039,
[3] = 27112052,
[4] = 3230472745,
[5] = 3230470862,
[6] = 1
},
[3] = "YinHub"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))

  end
})
AddButton(Main, {
  Name = "جسم قزم",
  Callback = function()
print("Clicked")local args = {
[1] = "CharacterChange",
[2] = {
[1] = 126267841602936,
[2] = 77530451194918,
[3] = 123471958406889,
[4] = 117042768644173,
[5] = 131948590344338,
[6] = 1
},
[3] = "YinHub"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))

  end
})
AddButton(Main, {
  Name = "هامستر جسم",
  Callback = function()
print("Clicked")local args = {
[1] = "CharacterChange",
[2] = {
[1] = 14898536974,
[2] = 14898536957,
[3] = 14898537277,
[4] = 14898537300,
[5] = 14898537292,
[6] = 14898536975,
},
[3] = "YinHub"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))

  end
})
AddButton(Main, {
  Name = "سيغما بوي",
  Callback = function()
print("Clicked")local args = {
[1] = "CharacterChange",
[2] = {
[1] = 18178775358,
[2] = 18178775182,
[3] = 18178775725,
[4] = 18178777453,
[5] = 18178775695,
[6] = 1
},
[3] = "YinHub"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))

  end
})
local Main = MakeTab({Name = "التنقلات "})
AddButton(Main, {
  Name = "أداه تنقل",
  Callback = function()
    local player = game.Players.LocalPlayer
    local mouse = player:GetMouse()

    local function createTeleportTool()
        local tool = Instance.new("Tool")
        tool.RequiresHandle = false
        tool.Name = "أداه تنقل"

        tool.Activated:Connect(function()
            local hitPos = mouse.Hit.p + Vector3.new(0, 2.5, 0)
            local pos = CFrame.new(hitPos)
            player.Character.HumanoidRootPart.CFrame = pos
        end)

        tool.Parent = player.Backpack
    end

    -- Cria a ferramenta inicialmente
    createTeleportTool()

    -- Adiciona a ferramenta novamente quando o personagem é reaparecido
    player.CharacterAdded:Connect(function()
        wait(0.1) -- Espera um curto período de tempo para garantir que o inventário seja carregado
        createTeleportTool()
    end)
  end
})

AddButton(Main, {
    Name = "لوحة 1",
    Callback = function()
        local plr = game.Players.LocalPlayer
        local char = plr.Character
        local hrp = char:FindFirstChild("HumanoidRootPart")

        if hrp then
            hrp.CFrame = CFrame.new(-242.68215942382812, 89.68680572509766, -549.6495361328125)
        else
            warn("HumanoidRootPart not found")
        end
    end
})

AddButton(Main, {
    Name = "لوحة 2",
    Callback = function()
        local plr = game.Players.LocalPlayer
        local char = plr.Character
        local hrp = char:FindFirstChild("HumanoidRootPart")

        if hrp then
            hrp.CFrame = CFrame.new(-630.480712890625, 26.586822509765625, 365.14093017578125)
        else
            warn("HumanoidRootPart not found")
        end
    end
})

-- Function to teleport to Teleport
local function teleportToGasStation()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(192, 4, 272)
end

AddButton(Main, {
    Name = "ورا البيوت",
    Description = "",
    Callback = teleportToGasStation
})

-- Function to teleport to Teleport
local function teleportToCenter()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(136, 4, 117)
end

AddButton(Main, {
    Name = "قدام البيوت",
    Description = "",
    Callback = teleportToCenter
})

-- Function to teleport to Criminal
local function teleportToCriminal()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-119, -28, 235)
end

AddButton(Main, {
    Name = "مكان أسلحة",
    Description = "Teleporta para as coordenadas do Criminal",
    Callback = teleportToCriminal
})

-- Function to teleport to House Abandoned
local function teleportToHouseAbandoned()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(986, 4, 63)
end

AddButton(Main, {
    Name = "بيت قفير",
    Description = "Teleporta para as coordenadas da Casa Abandonada",
    Callback = teleportToHouseAbandoned
})

-- Function to teleport to Portal Agency
local function teleportToPortalAgency()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(672, 4, -296)
end

AddButton(Main, {
    Name = "مكان سري",
    Description = "Teleporta para as coordenadas do Portal da Agência",
    Callback = teleportToPortalAgency
})

-- Function to teleport to Secret Location
local function teleportToSecretLocation()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(505, -75, 143)
end

AddButton(Main, {
    Name = "جو الأرض",
    Description = "Teleporta para as coordenadas do Local Secreto",
    Callback = teleportToSecretLocation
})

-- Function to teleport to School
local function teleportToSchool()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-312, 4, 211)
end

AddButton(Main, {
    Name = "مدرسة",
    Description = "Teleporta para as coordenadas da Escola",
    Callback = teleportToSchool
})

-- Function to teleport to Brooks Diner
local function teleportToBrooksDiner()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(161, 8, 52)
end

AddButton(Main, {
    Name = "قهوة",
    Description = "Teleporta para as coordenadas do Brooks Diner",
    Callback = teleportToBrooksDiner
})

local function teleportToBrooksDiner()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-26, 4, -23)
end

AddButton(Main, {
    Name = "البداية",
    Description = "Teleporta para as coordenadas do Brooks Diner",
    Callback = teleportToBrooksDiner
})


-- Function to teleport to Hospital
local function teleportToHospital()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-309, 4, 71)
end

AddButton(Main, {
    Name = "مستشفى",
    Description = "Teleporta para as coordenadas do Hospital",
    Callback = teleportToHospital
})

-- Function to teleport to Arch
local function teleportToArch()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-589, 141, -59)
end

AddButton(Main, {
    Name = "فوق الجسر",
    Description = "Teleporta para as coordenadas do Arco",
    Callback = teleportToArch
})

-- Function to teleport to Agency
local function teleportToAgency()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(179, 4, -464)
end

AddButton(Main, {
    Name = "مكان الكهرباء",
    Description = "Teleporta para as coordenadas da Agência",
    Callback = teleportToAgency
})

-- Function to teleport to Secret Room in Workshop
local function teleportToSecretRoomInWorkshop()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(0, 4, -495)
end

AddButton(Main, {
    Name = "جو الأرض",
    Description = "Teleporta para as coordenadas da Sala Secreta na Oficina",
    Callback = teleportToSecretRoomInWorkshop
})

-- Function to teleport to Secret Room 2
local function teleportToSecretRoom2()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-343, 4, -613)
end

AddButton(Main, {
    Name = "جو الأرض 2",
    Description = "Teleporta para as coordenadas da Sala Secreta 2",
    Callback = teleportToSecretRoom2
})

-- Function to teleport to Island 1
local function teleportToIsland1()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1925, 23, 127)
end

AddButton(Main, {
    Name = "جزيرة 1",
    Description = "Teleporta para as coordenadas da Ilha 1",
    Callback = teleportToIsland1
})

-- Function to teleport to Airport
local function teleportToAirport()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(310, 5, 31)
end

AddButton(Main, {
    Name = "مطار",
    Description = "Teleporta para as coordenadas do Aeroporto",
    Callback = teleportToAirport
})

-- Function to teleport to Hotel Center
local function teleportToHotelCenter()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(182, 4, 150)
end

AddButton(Main, {
    Name = "البيوت",
    Description = "Teleporta para as coordenadas do Centro dos Hotéis",
    Callback = teleportToHotelCenter
})

-- Function to teleport to Lower Houses
local function teleportToLowerHouses()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(63, 35, 410)
end

AddButton(Main, {
    Name = " نص الشارع",
    Description = "Teleporta para as coordenadas das Casas Inferiores",
    Callback = teleportToLowerHouses
})

-- Function to teleport to Mountain 1
local function teleportToMountain1()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-670, 251, 765)
end

AddButton(Main, {
    Name = "فوق الجبل",
    Description = "Teleporta para as coordenadas da Montanha 1",
    Callback = teleportToMountain1
})

-- Function to teleport to On Top of School
local function teleportToOnTopOfSchool()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-370, 50, 173)
end

AddButton(Main, {
    Name = "فوق المدرسة",
    Description = "Teleporta para as coordenadas Em Cima da Escola",
    Callback = teleportToOnTopOfSchool
})
local Main = MakeTab({Name = "تخريب"})

--[[
  Name = "Main" <string> Nome da guia
]]
MinimizeButton({
  Image = "rbxassetid://136300057076089",
  Size = {40, 40},
  Color = Color3.fromRGB(10, 10, 10),
  Corner = true,
  Stroke = true,
  StrokeColor = Color3.fromRGB(10, 10, 10)
})
local args = {
    [1] = "RolePlayName";
    [2] = "مطور سكربت EZ_HUB";
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
local args = {
    [1] = "RolePlayBio",
    [2] = "EZ_HUB"
}
game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
wait(0.1)
game.StarterGui:SetCore("SendNotification", {
    Title = "انتضر هسا يشتغل";
    Text = "سكربت مطور EZ"; -- ARAB TEAM
    Duration = 5;
})
wait(0.1)
game.StarterGui:SetCore("SendNotification", {
    Title = " لحضة ";
    Text = "جاري تحميل..."; -- ARAB TEAM
    Duration = 5;
})
local section = AddSection(Main, {"قتل سفينه"})
local Players = game:GetService("Players")
local LocalPlayer = Players.LocalPlayer

-- إنشاء قائمة بأسماء اللاعبين (ما عدا اللاعب المحلي)
local playerNames = {}
for _, plr in ipairs(Players:GetPlayers()) do
    if plr ~= LocalPlayer then
        table.insert(playerNames, plr.Name)
    end
end

local selectedPlayerName = nil

-- القائمة المنسدلة لاختيار اللاعب
local Dropdown = AddDropdown(Main, {
    Name = "اختر لاعب",
    Options = playerNames,
    Default = playerNames[1],
    Callback = function(Value)
        selectedPlayerName = Value
    end
})

-- زر التفعيل
AddButton(Main, {
    Name = "تفعيل",
    Callback = function()
        if not selectedPlayerName then
            warn("لم يتم اختيار لاعب")
            return
        end
MakeNotifi({
  Title = "تم التشغيل",
  Text = "عليك انتضار 13 ثواني حتى تفعل مرا اخرى",
  Time = 5
})

--[[
  Title = "REDz HUB" <string> titulo da notificação
  Text = "Notificação teste" <string> descrição da notificação
  Time = 5 <number> tempo da notificação
]]
        local targetPlayer = Players:FindFirstChild(selectedPlayerName)
        if targetPlayer and targetPlayer.Character and targetPlayer.Character:FindFirstChild("HumanoidRootPart") then
            local character = LocalPlayer.Character or LocalPlayer.CharacterAdded:Wait()
            local humanoid = character:WaitForChild("Humanoid")
            local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

            local originalPosition = humanoidRootPart.Position
            local originalAnchoredState = humanoidRootPart.Anchored

            humanoidRootPart.CFrame = CFrame.new(634.18, -4.00, 1839.65)
            wait(0.5)

            local args = {
                "PickingBoat",
                "MilitaryBoatFree"
            }
            game:GetService("ReplicatedStorage"):WaitForChild("RE"):WaitForChild("1Ca1r"):FireServer(unpack(args))
            wait(1.5)

            local function sitInBoat()
                local vehicle = workspace.Vehicles:FindFirstChild(LocalPlayer.Name .. "Car")
                if not vehicle then return end

                local vehicleSeat = vehicle.Body:FindFirstChild("VehicleSeat")
                if not vehicleSeat then return end

                humanoidRootPart.Anchored = false
                humanoid:ChangeState(Enum.HumanoidStateType.GettingUp)
                wait(0.2)

                humanoidRootPart.CFrame = vehicleSeat.CFrame * CFrame.new(0, 0.5, 0)
                wait(0.2)

                humanoid.Sit = true
                firetouchinterest(humanoidRootPart, vehicleSeat, 0)
                firetouchinterest(humanoidRootPart, vehicleSeat, 1)
                wait(0.5)

                if humanoid.SeatPart ~= vehicleSeat then
                    humanoidRootPart.CFrame = vehicleSeat.CFrame * CFrame.new(0, 0.5, 0)
                    humanoid.Sit = true
                    wait(0.5)
                end
            end

            sitInBoat()
            wait(0.5)

            local targetPosition = targetPlayer.Character.HumanoidRootPart.Position
            local vehicle = workspace.Vehicles:FindFirstChild(LocalPlayer.Name .. "Car")

            if vehicle then
                vehicle:SetPrimaryPartCFrame(CFrame.new(targetPosition + Vector3.new(0, -2, 0)))
                humanoidRootPart.CFrame = CFrame.new(targetPosition + Vector3.new(0, 5, 0))

                local crazyStart = tick()
                while tick() - crazyStart < 2 do
                    local offset = Vector3.new(
                        math.random(-8, 8),
                        math.random(-3, 1),
                        math.random(-8, 8)
                    )
                    vehicle:SetPrimaryPartCFrame(CFrame.new(targetPosition + Vector3.new(0, -2, 0) + offset))
                    wait(0.05)
                end
            end

            local targetDestination = Vector3.new(-86.00, -224.27, 34.57)
            if vehicle then
                vehicle:SetPrimaryPartCFrame(CFrame.new(targetDestination))
                humanoidRootPart.CFrame = CFrame.new(targetDestination + Vector3.new(0, 5, 0))
            end

            wait(0.5)
            humanoidRootPart.Anchored = false
            humanoid:ChangeState(Enum.HumanoidStateType.GettingUp)

            if vehicle then
                vehicle:Destroy()
            end

            wait(0.5)
            humanoidRootPart.CFrame = CFrame.new(originalPosition)
            humanoidRootPart.Anchored = originalAnchoredState
            humanoid:ChangeState(Enum.HumanoidStateType.RunningNoPhysics)
        else
            warn("اللاعب غير موجود أو لا يملك الشخصية")
        end
    end
})
local section = AddSection(Main, {"سوالف 🔞"})
local Players = game:GetService("Players")
local RunService = game:GetService("RunService")

local function fetchPlayerNames()
    local namesList = {}
    for _, plr in ipairs(Players:GetPlayers()) do
        if plr ~= Players.LocalPlayer then 
            table.insert(namesList, plr.Name)
        end
    end
    return namesList
end

local dropdown = AddDropdown(Main, {
    Name = "Select a player",
    Default = "...",
    Options = fetchPlayerNames(),
    Callback = function(Value)
        if Value ~= "" then
            getgenv().selectedPlayer = Value
        end
    end
})

local function createBangToggle(name, yOffset, faceBang)
    local bangActive = false
    local connection
    local togglePosition = false

    AddToggle(Main, {
        Name = name,
        Default = false,
        Callback = function(Value)
            bangActive = Value

            local player = Players.LocalPlayer
            local char = player.Character
            if not char then return end

            local humanoid = char:FindFirstChildOfClass("Humanoid")
            if not humanoid then return end

            if Value then
                humanoid.PlatformStand = true

                if connection then connection:Disconnect() end

                connection = RunService.Heartbeat:Connect(function()
                    if bangActive and getgenv().selectedPlayer then
                        local targetPlayer = Players:FindFirstChild(getgenv().selectedPlayer)
                        if targetPlayer and targetPlayer.Character and targetPlayer.Character.PrimaryPart then
                            local targetHead = targetPlayer.Character:FindFirstChild("Head")
                            if targetHead and char.PrimaryPart then
                                local offset = togglePosition and 1 or 4
                                if faceBang then
                                    char:SetPrimaryPartCFrame(targetHead.CFrame * CFrame.new(0, 1, -offset) * CFrame.Angles(0, math.rad(180), 0))
                                else
                                    char:SetPrimaryPartCFrame(targetHead.CFrame * CFrame.new(0, yOffset, offset) * CFrame.Angles(0, 0, 0))
                                end
                                togglePosition = not togglePosition
                                wait(1)
                            end
                        end
                    end
                end)
            else
                humanoid.PlatformStand = false
                if connection then
                    connection:Disconnect()
                    connection = nil
                end
            end
        end    
    })
end

createBangToggle("Bang", -1, false)
createBangToggle("Bang 2", -1.5, false)
createBangToggle("الوجه Bang", 1, true)
createBangToggle("الوجه Bang 2", 1, true)
local Main = MakeTab({Name = "أسماء"})

--[[
  Name = "Main" <string> Nome da guia
]]
AddButton(Main, {
  Name = "ليو",
  Callback = function()
    local args = {
    [1] = "RolePlayName",
    [2] = "لــَيو"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "عبد الله ",
  Callback = function()
    local args = {
    [1] = "RolePlayName",
    [2] = "عبــدُ الـُلَه"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "عباس",
  Callback = function()
    local args = {
    [1] = "RolePlayName",
    [2] = "عبــوصـُ"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "يمان",
  Callback = function()
    local args = {
    [1] = "RolePlayName",
    [2] = "يمان"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "محمد",
  Callback = function()
    local args = {
    [1] = "RolePlayName",
    [2] = "محمدُ"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "دراجون",
  Callback = function()
    local args = {
    [1] = "RolePlayName",
    [2] = "دراجَونـ"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "حمود",
  Callback = function()
    local args = {
    [1] = "RolePlayName",
    [2] = "حـمـُود"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "حسين",
  Callback = function()
    local args = {
    [1] = "RolePlayName",
    [2] = "حـَسينُ"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "امجد",
  Callback = function()
    local args = {
    [1] = "RolePlayName",
    [2] = "أمـجـُد "
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
  end
})
local section = AddSection(Main, {"أسماء بنات"})
AddButton(Main, {
  Name = "جنى",
  Callback = function()
    local args = {
    [1] = "RolePlayName",
    [2] = "JANA"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "ليسى",
  Callback = function()
    local args = {
    [1] = "RolePlayName",
    [2] = "Lacey"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "نور",
  Callback = function()
    local args = {
    [1] = "RolePlayName",
    [2] = "noor"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "ليلى",
  Callback = function()
    local args = {
    [1] = "RolePlayName",
    [2] = "Layla"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "فاطمه",
  Callback = function()
    local args = {
    [1] = "RolePlayName",
    [2] = "Fatima"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "تالين",
  Callback = function()
    local args = {
    [1] = "RolePlayName",
    [2] = "Tallinn"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "مالك",
  Callback = function()
    local args = {
    [1] = "RolePlayName",
    [2] = "MALAK"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args))
  end
})
local Main = MakeTab({Name = "البيت"})

--[[
  Name = "البيت" <string> Nome da guia
]]
AddButton(Main, {
  Name = "1 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "2 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 2
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "3 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 3
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "4 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 4
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "5 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 5
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "6 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 6
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "7 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 7
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "11 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 11
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "12 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 12
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "13 تاخذ تحكم البيت ",
  Callback = function()
    	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 13
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "14 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 14
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "15 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 15
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "16 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 16
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "17 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 17
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "18 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 18
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "19 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 19
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "20 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 20
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "21 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 21
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "22 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 22
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
AddButton(Main, {
  Name = "23 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 23
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))
  end
})
AddButton(Main, {
  Name = "24 تاخذ تحكم البيت ",
  Callback = function()
    local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 24
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  end
})
local Main = MakeTab({Name = "شغلات جانبيه"})

--[[
  Name = "Main" <string> Nome da guia
]]
AddTextBox(Main, {
  Name = "سرعة | Speed",
  Default = "",
  PlaceholderText = "ادخل رقم",
  ClearText = true,
  Callback = function(value)
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = value     
 end
})
AddTextBox(Main, {
  Name = "قفز | Jump",
  Default = "",
  PlaceholderText = "ادخل رقم",
  ClearText = true,
  Callback = function(value)
game.Players.LocalPlayer.Character.Humanoid.JumpPower = value    
  end
})
AddTextBox(Main, {
  Name = "Fov | شاشه",
  Default = "",
  PlaceholderText = "ادخل رقم",
  ClearText = true,
  Callback = function(value)
local FovNumber = value
local Camera = workspace.CurrentCamera
Camera.FieldOfView = FovNumber  
  end
})
AddTextBox(Main, {
  Name = "Spin | دوران",
  Default = "",
  PlaceholderText = "ادخل رقم",
  ClearText = true,
  Callback = function(Value)
    getgenv().Spinspeed = Value

local Spin = Instance.new'BodyAngularVelocity'
Spin.Parent = game:GetService'Players'.LocalPlayer.Character:FindFirstChild'HumanoidRootPart'
Spin.MaxTorque = Vector3.new(0, math.huge, 100)
wait(0.1)
Spin.AngularVelocity = Vector3.new(100,Spinspeed,0)
  end
})
AddButton(Main, {
  Name = "كنبه | Couch",
  Callback = function()
    local args={[1]="PickingTools",[2]="Couch"};game:GetService("ReplicatedStorage").RE:FindFirstChild("1Too1l"):InvokeServer(unpack(args))
  end
})
local infiniteJumpEnabled = false

-- Conectar o evento de pulo somente uma vez
local infiniteJumpConnection

-- Função de callback para o botão de alternância de pulo infinito
local function onInfiniteJumpToggle(value)
    infiniteJumpEnabled = value
    print("Infinite Jump Enabled:", infiniteJumpEnabled)
    
    -- Conectar o evento de pulo somente uma vez
    if not infiniteJumpConnection then
        infiniteJumpConnection = game:GetService("UserInputService").JumpRequest:Connect(function()
            if infiniteJumpEnabled then
                local player = game.Players.LocalPlayer
                local character = player.Character
                if character and character:FindFirstChildOfClass("Humanoid") then
                    character:FindFirstChildOfClass("Humanoid"):ChangeState("Jumping")
                end
            end
        end)
    end
end

-- Adiciona o botão de alternância "Infinitejum    
    local Toggle = AddToggle(Main, {
    Name = "قفز لا نهائي | Inf Jump",
    Default = false,
    Callback = onInfiniteJumpToggle
})
function MakeNotifi(notification)
    game.StarterGui:SetCore("SendNotification", {
        Title = notification.Title;
        Text = notification.Text;
        Duration = notification.Time;
    })
end
function MakeNotifi(notification)
    game.StarterGui:SetCore("SendNotification", {
        Title = notification.Title;
        Text = notification.Text;
        Duration = notification.Time;
    })
end

-- Variáveis e funções para a visualização dos jogadores
local viewEnabled = false
local selectedViewPlayer = nil
local characterAddedConnection = nil

local function toggleView(enabled)
    if enabled then
        if selectedViewPlayer then
            local player = selectedViewPlayer
            if player then
                game.Workspace.CurrentCamera.CameraSubject = player.Character
                if characterAddedConnection then
                    characterAddedConnection:Disconnect()
                end
                characterAddedConnection = player.CharacterAdded:Connect(function(character)
                    game.Workspace.CurrentCamera.CameraSubject = character
                end)
                MakeNotifi({
                    Title = "Visualizando " .. player.Name,
                    Text = "Você está visualizando o jogador: " .. player.Name,
                    Time = 6
                })
            else
                print("Jogador não encontrado.")
                viewEnabled = false
            end
        else
            print("Nenhum jogador selecionado para a visualização.")
            viewEnabled = false
        end
    else
        if characterAddedConnection then
            characterAddedConnection:Disconnect()
            characterAddedConnection = nil
        end
        game.Workspace.CurrentCamera.CameraSubject = game.Players.LocalPlayer.Character
    end
end

local value = "" -- Variável para armazenar o nome digitado

local function findPlayerByPartialNameOrNickname(partialName)
    value = partialName -- Atualiza a variável com o nome digitado completo
    for _, player in ipairs(game.Players:GetPlayers()) do
        if player.Name:lower():find(partialName:lower(), 1, true) or (player.DisplayName and player.DisplayName:lower():find(partialName:lower(), 1, true)) then
            return player
        end
    end
    return nil
end

-- Adicionando a caixa de texto para entrada do nome ou apelido do jogador
local Main = MakeTab({Name = "HUNT EGG"})

--[[
  Name = "Main" <string> Nome da guia
]]
local Paragraph = AddParagraph(Main, {"قبل لاتشغل سكربت اختار مهمه ياحبيبي"})

local Toggle = AddToggle(Main, {
  Name = "تجميع بيض",
  Default = false,
  Callback = function(Value)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
    
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
    
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
    
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
        
    wait(0.5)
    game:GetService("ReplicatedStorage").Remotes.EggCollected:InvokeServer()
    
  end
})

--[[
  Name = "Toggle teste" <string> nome da sua caixa de seleção
  Default = false <boolean> valor padrão
  Callback = function(Value)
    -- função da sua caixa de seleção
  end
]]
