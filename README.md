












_G.Auto_Kaitun = true

if not game:IsLoaded() then game.Loaded:Wait() end
repeat wait() until game.Players
repeat wait() until game.Players.LocalPlayer
repeat wait() until game.ReplicatedStorage
repeat wait() until game.ReplicatedStorage:FindFirstChild("Remotes");
repeat wait() until game.Players.LocalPlayer:FindFirstChild("PlayerGui");
repeat wait() until game.Players.LocalPlayer.PlayerGui:FindFirstChild("Main");

wait(1)


if not game:IsLoaded() then repeat game.Loaded:Wait() until game:IsLoaded() end

if game:GetService("Players").LocalPlayer.PlayerGui.Main:FindFirstChild("ChooseTeam") then
    repeat wait()
        if game:GetService("Players").LocalPlayer.PlayerGui:WaitForChild("Main").ChooseTeam.Visible == true then
            for i, v in pairs(getconnections(game:GetService("Players").LocalPlayer.PlayerGui.Main.ChooseTeam.Container.Pirates.Frame.TextButton.Activated)) do                                                                                                
                v.Function()
            end
        end
    until game.Players.LocalPlayer.Team ~= nil and game:IsLoaded()
end






if game.PlaceId == 2753915549 then
    OLD_World = true
end



function code(x)
    game:GetService("ReplicatedStorage").Remotes.Redeem:InvokeServer(x)
end






if OLD_World then
    code("FIGHT4FRUIT")
    code("NOEXPLOIT")
    code("NOOB2ADMIN")
    code("CODESLIDE")
    code("ADMINDARES")
    code("ZIOLES")
    code("TRIPLEABUSE")
    code("SEATROLLING")
    code("24NOADMIN")
    code("NewtRoll")
    code("Bluxxy")
    code("KittGaming")
    code("Enyu_is_Pro")
    code("MagicBus")
    code("JCWK")
    code("StarcodeHEO")
    code("Sub2Fer999")
    code("Sub2CaptainMaui")
    code("Sub2GamerRobot_EXP1")
    code("Sub2NoobMaster123")
    code("Sub2Daigrock")
    code("Sub2OfficialNoobie")
    code("Bluxxy")
    code("Axiore")
    code("TantaiGaming")
    code("StrawHatMaine")
    code("BigNews")
    code("TheGreatAce")
    if game.Players.LocalPlayer.PlayerGui:FindFirstChild("Notifications") then
        game.Players.LocalPlayer.PlayerGui:FindFirstChild("Notifications").Enabled = false
    end

end


-- game.Players.LocalPlayer.PlayerGui.Notification.Enabled = false











-- game:GetService("Players").PlayerAdded:Connect(function()
--     table.clear(ply_list)
--     for i,v in pairs(game:GetService("Players"):GetPlayers()) do
--         if v.Name ~= LocalPlayer.Name then
--             table.insert(ply_list,v.Name)
--         end
--     end
-- end)

-- game:GetService("Players").PlayerRemoving:Connect(function()
--     table.clear(ply_list)
--     for i,v in pairs(game:GetService("Players"):GetPlayers()) do
--         if v.Name ~= LocalPlayer.Name then
--             table.insert(ply_list,v.Name)
--         end
--     end
-- end)


---- Check  Kaitun
spawn(function()
    while wait() do
        if _G.Auto_Kaitun then
            pcall(function()
                game.Players.LocalPlayer.Character.Humanoid.Sit = false
                if OLD_World then
                    Kaitun_FirstSea = true
                end
            end)
        end
    end
end)





function checklv()
    local MYLEVEL = game:GetService("Players").LocalPlayer.Data.Level.Value
    if OLD_World then
        if  MYLEVEL == 1 or MYLEVEL <= 9 then
            NameMon = "Bandit"
            NameQ = "BanditQuest1"
            Lvq = 1
            POSMON = CFrame.new(967.5056762695312, 16.349260330200195, 1549.0823974609375)
            POSQuest = CFrame.new(1062.026123046875, 16.362735748291016, 1549.199951171875)
        elseif MYLEVEL == 10 or MYLEVEL <= 14 then
            NameMon = "Monkey"
            NameQ = "JungleQuest"
            Lvq = 1
            POSMON = CFrame.new(-1609.71216, 39.8521576, 123.384674, 0.708323717, 6.74341152e-08, 0.705887735, -1.86098941e-08, 1, -7.68568071e-08, -0.705887735, 4.13030072e-08, 0.708323717)
            POSQuest = CFrame.new(-1600.24353, 36.8521347, 153.224792, 0.0664860159, 1.09421023e-07, -0.997787356, 9.55680779e-09, 1, 1.10300476e-07, 0.997787356, -1.68691017e-08, 0.0664860159)
        elseif MYLEVEL == 15 or MYLEVEL <= 29 then
            NameQ = "JungleQuest"
            Lvq = 2
            NameMon = "Gorilla"
            POSQuest = CFrame.new(-1600.24353, 36.8521347, 153.224792, 0.0664860159, 1.09421023e-07, -0.997787356, 9.55680779e-09, 1, 1.10300476e-07, 0.997787356, -1.68691017e-08, 0.0664860159)
            POSMON = CFrame.new(-1260.29321, 18.6214619, -398.3508, 0.816335142, 5.76316722e-07, -0.577578545, 8.32609999e-08, 1, 1.11549434e-06, 0.577578545, -9.58707005e-07, 0.816335142)
        elseif MYLEVEL == 30 or MYLEVEL <= 39 then
            NameQ = "BuggyQuest1"
            Lvq = 1
            NameMon = "Pirate"
            POSQuest = CFrame.new(-1139.56116, 4.75204945, 3825.97827, -0.947666645, 2.60038924e-08, 0.319261551, 3.65571005e-08, 1, 2.70626153e-08, -0.319261551, 3.73176157e-08, -0.947666645)
            POSMON = CFrame.new(-1223.64111, 4.75204945, 3914.84668, -0.99005419, 5.39223821e-09, 0.140686572, -6.35229591e-10, 1, -4.27983267e-08, -0.140686572, -4.24620303e-08, -0.99005419)
        elseif MYLEVEL == 40 or MYLEVEL <= 59 then
            NameQ = "BuggyQuest1"
            Lvq = 2
            NameMon = "Brute"
            POSQuest = CFrame.new(-1139.56116, 4.75204945, 3825.97827, -0.947666645, 2.60038924e-08, 0.319261551, 3.65571005e-08, 1, 2.70626153e-08, -0.319261551, 3.73176157e-08, -0.947666645)
            POSMON = CFrame.new(-1140.92944, 14.8098745, 4317.16455, -0.943479657, 3.71900555e-08, -0.331430465, 1.7316566e-08, 1, 6.2915845e-08, 0.331430465, 5.36205853e-08, -0.943479657)
        elseif MYLEVEL == 60 or MYLEVEL <= 74 then
            NameQ = "DesertQuest"
            Lvq = 1
            NameMon = "Desert Bandit"
            POSQuest = CFrame.new(896.408142, 6.43846178, 4389.37891, -0.846945703, -2.31297754e-08, 0.531679392, -1.55507234e-08, 1, 1.87315088e-08, -0.531679392, 7.59657048e-09, -0.846945703)
            POSMON = CFrame.new(949.532593, 15.2893953, 4403.09912, -0.832314849, -4.19622452e-08, 0.55430311, 7.94023236e-10, 1, 7.68949704e-08, -0.55430311, 6.44409539e-08, -0.832314849)
        elseif MYLEVEL == 75 or MYLEVEL <= 89 then
            NameQ = "DesertQuest"
            Lvq = 2
            NameMon = "Desert Officer"
            POSQuest = CFrame.new(896.408142, 6.43846178, 4389.37891, -0.846945703, -2.31297754e-08, 0.531679392, -1.55507234e-08, 1, 1.87315088e-08, -0.531679392, 7.59657048e-09, -0.846945703)
            POSMON = CFrame.new(1547.40369, 14.4520388, 4359.40625, 0.228631318, -1.20783e-07, -0.973513126, -3.43095508e-08, 1, -1.32126871e-07, 0.973513126, 6.36091286e-08, 0.228631318)
        elseif MYLEVEL == 90 or MYLEVEL <= 99 then
            NameQ = "SnowQuest"
            Lvq = 1
            NameMon = "Snow Bandit"
            POSQuest = CFrame.new(1384.01538, 87.272789, -1296.28137, 0.462413222, -7.79864777e-08, -0.88666451, -1.42050363e-08, 1, -9.53630916e-08, 0.88666451, 5.6692258e-08, 0.462413222)
            POSMON = CFrame.new(1372.84326, 105.990303, -1422.19507, 0.719091773, -2.12436309e-08, 0.694915235, 9.82151036e-08, 1, -7.10619616e-08, -0.694915235, 1.19351228e-07, 0.719091773)
        elseif MYLEVEL == 100 or MYLEVEL <= 119 then
            NameQ = "SnowQuest"
            Lvq = 2
            NameMon = "Snowman"
            POSQuest = CFrame.new(1384.01538, 87.272789, -1296.28137, 0.462413222, -7.79864777e-08, -0.88666451, -1.42050363e-08, 1, -9.53630916e-08, 0.88666451, 5.6692258e-08, 0.462413222)
            POSMON = CFrame.new(1220.92712, 138.011871, -1489.01208, 0.389352709, -7.53626693e-07, 0.921088696, 1.45705499e-07, 1, 7.56600116e-07, -0.921088696, -1.60376572e-07, 0.389352709)
        elseif MYLEVEL == 120 or MYLEVEL <= 149 then
            NameQ = "MarineQuest2"
            Lvq = 1
            NameMon = "Chief Petty Officer"
            POSQuest = CFrame.new(-5034.64893, 28.6520348, 4324.53369, -0.0616381466, 5.83357576e-08, 0.998098552, -1.59750098e-08, 1, -5.9433436e-08, -0.998098552, -1.96080023e-08, -0.0616381466)
            POSMON = CFrame.new(-4863.61328, 22.6520348, 4306.39307, 0.536051273, 7.00434066e-09, -0.844185412, -5.8011751e-10, 1, 7.92878918e-09, 0.844185412, -3.76051057e-09, 0.536051273)
        elseif MYLEVEL == 150 or MYLEVEL <= 174 then
            NameQ = "SkyQuest"
            Lvq = 1
            NameMon = "Sky Bandit"
            POSQuest = CFrame.new(-4843.2041, 717.669617, -2623.13159, -0.775086224, -1.6359829e-08, -0.631855488, -4.10942462e-08, 1, 2.45178793e-08, 0.631855488, 4.49690951e-08, -0.775086224)
            POSMON = CFrame.new(-4970.74219, 294.544342, -2890.11353, -0.994874597, -8.61311165e-08, -0.101116329, -9.10836278e-08, 1, 4.43614923e-08, 0.101116329, 5.33441664e-08, -0.994874597)
        elseif MYLEVEL == 175 or MYLEVEL <= 189 then
            NameQ = "SkyQuest"
            Lvq = 2
            NameMon = "Dark Master"
            POSQuest = CFrame.new(-4843.2041, 717.669617, -2623.13159, -0.775086224, -1.6359829e-08, -0.631855488, -4.10942462e-08, 1, 2.45178793e-08, 0.631855488, 4.49690951e-08, -0.775086224)
            POSMON = CFrame.new(-5239.94629, 392.217102, -2208.18335, 0.969297886, -5.95604988e-09, -0.245889395, 3.87897714e-09, 1, -8.93151775e-09, 0.245889395, 7.70350184e-09, 0.969297886)
        elseif MYLEVEL == 190 or MYLEVEL <= 209 then
            NameQ = "PrisonerQuest"
            Lvq = 1
            NameMon = "Prisoner"
            POSQuest = CFrame.new(5307.95166015625, 1.6809712648391724, 475.1698913574219)
            POSMON = CFrame.new(5029.708984375, 68.67806243896484, 445.857177734375)
        elseif MYLEVEL == 210 or MYLEVEL <= 249 then
            NameQ = "PrisonerQuest"
            Lvq = 2
            NameMon = "Dangerous Prisoner"
            POSQuest = CFrame.new(5307.95166015625, 1.6809712648391724, 475.1698913574219)
            POSMON = CFrame.new(5673.51758, 68.6786652, 783.757629, -0.0514698699, 7.78369369e-08, 0.998674572, 8.35602094e-08, 1, -7.36337e-08, -0.998674572, 7.96595359e-08, -0.0514698699)
        elseif MYLEVEL == 250 or MYLEVEL <= 274 then
            NameQ = "ColosseumQuest"
            Lvq = 1
            NameMon = "Toga Warrior"
            POSQuest = CFrame.new(-1575.72961, 7.38933659, -2983.39453, 0.52762109, -1.48187587e-06, 0.849479854, 2.69328297e-07, 1, 1.57716818e-06, -0.849479854, -6.0335816e-07, 0.52762109)
            POSMON = CFrame.new(-1819.12415, 7.28907108, -2744.02539, 0.547199547, 2.10840998e-08, -0.837002158, -1.27399286e-10, 1, 2.51067309e-08, 0.837002158, -1.36317579e-08, 0.547199547)
        elseif MYLEVEL == 275 or MYLEVEL <= 299 then
            NameQ = "ColosseumQuest"
            Lvq = 2
            NameMon = "Gladiator"
            POSQuest = CFrame.new(-1575.72961, 7.38933659, -2983.39453, 0.52762109, -1.48187587e-06, 0.849479854, 2.69328297e-07, 1, 1.57716818e-06, -0.849479854, -6.0335816e-07, 0.52762109)
            POSMON = CFrame.new(-1334.76514, 7.44254398, -3228.90552, -0.340173125, 2.8230156e-08, 0.940362811, 2.60959143e-09, 1, -2.90764834e-08, -0.940362811, -7.4370754e-09, -0.340173125)
        elseif MYLEVEL == 300 or MYLEVEL <= 324 then
            NameQ = "MagmaQuest"
            Lvq = 1
            NameMon = "Military Soldier"
            POSQuest = CFrame.new(-5316.33887, 12.236989, 8517.67285, 0.499506682, -5.08374072e-08, -0.86631006, -1.30872131e-08, 1, -6.62286652e-08, 0.86631006, 4.44192452e-08, 0.499506682)
            POSMON = CFrame.new(-5419.0752, 10.9255161, 8464.50488, -0.637788415, -4.55103836e-05, 0.770211577, 7.05542743e-06, 1, 6.49305366e-05, -0.770211577, 4.68461185e-05, -0.637788415)
        elseif MYLEVEL == 325 or MYLEVEL <= 374 then
            NameQ = "MagmaQuest"
            Lvq = 2
            NameMon = "Military Spy"
            POSQuest = CFrame.new(-5316.33887, 12.236989, 8517.67285, 0.499506682, -5.08374072e-08, -0.86631006, -1.30872131e-08, 1, -6.62286652e-08, 0.86631006, 4.44192452e-08, 0.499506682)
            POSMON = CFrame.new(-5805.42041, 99.5276108, 8782.36719, -0.316935152, -6.4923519e-08, 0.948447227, 4.12987404e-08, 1, 8.2252896e-08, -0.948447227, 6.52385026e-08, -0.316935152)
        elseif MYLEVEL == 375 or MYLEVEL <= 399 then
            NameQ = "FishmanQuest"
            Lvq = 1
            NameMon = "Fishman Warrior"
            POSQuest = CFrame.new(61122.2422, 18.4716377, 1568.84778, 0.971045971, -1.77007031e-08, 0.238892734, 4.80190776e-09, 1, 5.45760841e-08, -0.238892734, -5.18487475e-08, 0.971045971)
            POSMON = CFrame.new(60898.043, 18.4828224, 1550.9906, -0.0750192106, -4.46996573e-09, 0.997182071, 3.6461556e-10, 1, 4.51002746e-09, -0.997182071, 7.0192685e-10, -0.0750192106)
            if Auto_Farm_LV and (POSQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 3000 then
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
            end
        elseif MYLEVEL == 400 or MYLEVEL <= 449 then
            NameQ = "FishmanQuest"
            Lvq = 2
            NameMon = "Fishman Commando"
            POSQuest = CFrame.new(61122.2422, 18.4716377, 1568.84778, 0.971045971, -1.77007031e-08, 0.238892734, 4.80190776e-09, 1, 5.45760841e-08, -0.238892734, -5.18487475e-08, 0.971045971)
            POSMON = CFrame.new(61885.4063, 18.4828224, 1500.37195, 0.722261012, 4.84021889e-08, -0.691620588, 1.27929427e-08, 1, 8.33434299e-08, 0.691620588, -6.90435726e-08, 0.722261012)
            if Auto_Farm_LV and (POSQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 3000 then
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
            end
        elseif MYLEVEL == 450 or MYLEVEL <= 474 then
            NameQ = "SkyExp1Quest"
            Lvq = 1
            NameMon = "God's Guard"
            POSQuest = CFrame.new(-4721.28369, 845.277161, -1954.95154, -0.979754269, -1.72096932e-08, 0.200205252, -2.52417198e-09, 1, 7.36076018e-08, -0.200205252, 7.16119786e-08, -0.979754269)
            POSMON = CFrame.new(-4630.00635, 866.902954, -1936.76331, -0.656243384, 9.12737941e-12, 0.754549265, 3.58402819e-09, 1, 3.10498938e-09, -0.754549265, 4.74195483e-09, -0.656243384)
            if Auto_Farm_LV and (POSQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 3000 then
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-4607.82275, 872.54248, -1667.55688))
            end
        elseif MYLEVEL == 475 or MYLEVEL <= 524 then
            NameQ = "SkyExp1Quest"
            Lvq = 2
            NameMon = "Shanda"
            POSQuest = CFrame.new(-7861.79736, 5545.49316, -379.920776, 0.504107952, -1.41941534e-08, -0.863640666, -1.31181936e-08, 1, -2.40923566e-08, 0.863640666, 2.34745521e-08, 0.504107952)
            POSMON = CFrame.new(-7682.69775, 5607.36279, -445.691833, 0.786274791, -4.48163426e-08, -0.617877364, -4.81674345e-09, 1, -7.86622607e-08, 0.617877364, 6.48263239e-08, 0.786274791)
            if Auto_Farm_LV and (POSQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 3000 then
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-7894.6176757813, 5547.1416015625, -380.29119873047))
            end
        elseif MYLEVEL == 525 or MYLEVEL <= 549 then
            NameQ = "SkyExp2Quest"
            Lvq = 1
            NameMon = "Royal Squad"
            POSQuest = CFrame.new(-7902.23242, 5635.96387, -1411.96741, -0.0435957126, -2.13718043e-09, 0.999049246, 4.23562352e-10, 1, 2.15769735e-09, -0.999049246, 5.1722604e-10, -0.0435957126)
            POSMON = CFrame.new(-7579.42285, 5628.39111, -1540.75073, -0.0374937952, 1.17099557e-08, 0.999296963, -3.30279164e-08, 1, -1.29574085e-08, -0.999296963, -3.34905081e-08, -0.0374937952)
        elseif MYLEVEL == 550 or MYLEVEL <= 624 then
            NameQ = "SkyExp2Quest"
            Lvq = 2
            NameMon = "Royal Soldier"
            POSQuest = CFrame.new(-7902.23242, 5635.96387, -1411.96741, -0.0435957126, -2.13718043e-09, 0.999049246, 4.23562352e-10, 1, 2.15769735e-09, -0.999049246, 5.1722604e-10, -0.0435957126)
            POSMON = CFrame.new(-7834.84717, 5681.36182, -1790.76782, -0.102890432, 3.28112684e-08, 0.994692683, -6.45397762e-08, 1, -3.96622966e-08, -0.994692683, -6.82781121e-08, -0.102890432)
        elseif MYLEVEL == 625 or MYLEVEL <= 649 then
            NameQ = "FountainQuest"
            Lvq = 1
            NameMon = "Galley Pirate"
            POSQuest = CFrame.new(5254.52734, 38.5011368, 4049.80127, -0.0732342899, 2.23174847e-08, -0.997314751, 1.2052287e-07, 1, 1.35274023e-08, 0.997314751, -1.19208565e-07, -0.0732342899)
            POSMON = CFrame.new(5597.58936, 41.5013657, 3960.55371, -0.584786832, 4.98908861e-08, 0.811187029, 4.10757259e-08, 1, -3.18919575e-08, -0.811187029, 1.4670098e-08, -0.584786832)
        elseif MYLEVEL >= 650 then
            NameQ = "FountainQuest"
            Lvq = 2
            NameMon = "Galley Captain"
            POSQuest = CFrame.new(5254.52734, 38.5011368, 4049.80127, -0.0732342899, 2.23174847e-08, -0.997314751, 1.2052287e-07, 1, 1.35274023e-08, 0.997314751, -1.19208565e-07, -0.0732342899)
            POSMON = CFrame.new(5705.8252, 52.241478, 4890.11035, -0.969319642, 4.40228476e-09, 0.245803744, -7.88622412e-09, 1, -4.90088397e-08, -0.245803744, -4.94436954e-08, -0.969319642)    
        end
    end
end





function CheckWp(Get)
    for i,v in pairs(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("getInventory")) do
        if type(v) == "table" then
            if (v.Type == "Sword" or v.Type == "Gun" or v.Type == "Wear") and v.Name == Get then
                return true  -- คืนค่า true ถ้าเจอไอเท็มที่ต้องการ
            end
        end
    end
    return false 
end







-- First Sea
-- spawn(function()
--     while wait() do
--         if Kaitun_FirstSea then
--             pcall(function()
--                 local LV = game:GetService("Players").LocalPlayer.Data.Level.Value
--                 ---------------------------------    AutoFarm LV  ---------------------------
--                 if LV <= 15 then
--                     if  game.Players.LocalPlayer.Character.Humanoid.Health  > 0 then
--                         if game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false then
--                             checklv()
--                             repeat wait()
--                                 local distance_quest = (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - POSQuest.Position).magnitude
--                                 if distance_quest <= 5 then
--                                     wait(.5)
--                                     game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest",NameQ,Lvq)
--                                 else
--                                     TP(POSQuest)
--                                 end
--                             until   game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true or not Kaitun_FirstSea
--                     elseif game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true then
--                             checklv()
--                             if not string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text,NameMon) then
--                                 game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
--                             end
--                             if game:GetService("Workspace").Enemies:FindFirstChild(NameMon) then
--                                 for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
--                                     if v:FindFirstChild('Humanoid')  and  v:FindFirstChild('HumanoidRootPart') then
--                                         if v.Name == NameMon then
--                                             repeat wait()
--                                                     if not game.Players.LocalPlayer.Character:FindFirstChild('HasBuso') then
--                                                         game.ReplicatedStorage.Remotes.CommF_:InvokeServer('Buso')
--                                                     end
--                                                     StartMagnet = true
--                                                     TP(v.HumanoidRootPart.CFrame * CFrame.new(0,30,0))
--                                                     v.HumanoidRootPart.Size = Vector3.new(60,60,60)
--                                                     v.HumanoidRootPart.Transparency = 1
--                                                     v.Humanoid.JumpPower = 0
--                                                     v.Humanoid.WalkSpeed = 0
--                                                     v.HumanoidRootPart.CanCollide = false
--                                                     v.Humanoid:ChangeState(11)
--                                                     v.Humanoid:ChangeState(14)
--                                                     Pos_Mon = v.HumanoidRootPart.CFrame
--                                                     click()
--                                             until  v.Humanoid.Health <= 0 or not v.Parent or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false or not Kaitun_FirstSea
--                                             StartMagnet = false
--                                         end
--                                     end
--                                 end
--                             elseif not game:GetService("Workspace").Enemies:FindFirstChild(NameMon) then
--                                 TP(POSMON)
--                             end
--                         end
--                     end
--                 ---------------------------------   Auto Shanda  ---------------------------
--                 elseif LV == 16 or LV <= 60 then
--                     local Puk_Mon = CFrame.new(-7682.69775, 5607.36279, -445.691833, 0.786274791, -4.48163426e-08, -0.617877364,-4.81674345e-09, 1, -7.86622607e-08, 0.617877364, 6.48263239e-08, 0.786274791)
--                     if game:GetService("Workspace").Enemies:FindFirstChild("Shanda") then
--                         for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
--                             if v:FindFirstChild('Humanoid')  and  v:FindFirstChild('HumanoidRootPart') then
--                                 if v.Name == "Shanda" then
--                                     repeat wait()
--                                         if not game.Players.LocalPlayer.Character:FindFirstChild('HasBuso') then
--                                             game.ReplicatedStorage.Remotes.CommF_:InvokeServer('Buso')
--                                         end
--                                         StartMagnet_Fast = true
--                                         TP(v.HumanoidRootPart.CFrame * CFrame.new(0,30,0))
--                                         v.HumanoidRootPart.Size = Vector3.new(60,60,60)
--                                         v.HumanoidRootPart.Transparency = 1
--                                         v.Humanoid.JumpPower = 0
--                                         v.Humanoid.WalkSpeed = 0
--                                         v.HumanoidRootPart.CanCollide = false
--                                         v.Humanoid:ChangeState(11)
--                                         v.Humanoid:ChangeState(14)
--                                         Pos_Mon = v.HumanoidRootPart.CFrame
--                                         click()
--                                     until Kaitun_FirstSea == false  or v.Humanoid.Health <= 0 or not v.Parent or game.Players.LocalPlayer.Data.Level.Value > 60
--                                     StartMagnet_Fast = false
--                                 end
--                             end
--                         end
--                     elseif not game:GetService("Workspace").Enemies:FindFirstChild("Shanda") then
--                         if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Puk_Mon.Position).magnitude > 3000 then
--                             game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-7894.6176757813, 5547.1416015625, -380.29119873047))
--                         else
--                             TP(Puk_Mon)
--                         end
--                     end
--                 ------------------------------------   Auto Farm Hunter  --------------------------------------
--                 elseif LV == 61 or LV <= 200 then
--                     local ply = game.Players:GetPlayers()
--                     local = quest_title = game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text
--                     -- ------------------------------------   If Player have only me or Playerhunter Quest Can  not do  --------------------------------------
--                     local quest_hun = game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("PlayerHunter")
--                     if game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true and (#ply-1) != 0 and string.find(quest_title, "Defeat") and string.find(quest_title, "(0/1)" then
--                         print("1")
--                     end        
--                 end
--             end)
--         end
--     end
-- end)



function TP(P)
    Distance = (P.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
    if Distance < 10 then
        Speed = 1000
    elseif Distance < 170 then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = P
        Speed = 350
    elseif Distance < 1000 then
        Speed = 350
    elseif Distance >= 1000 then
        Speed = 250
    end
    game:GetService("TweenService"):Create(
        game.Players.LocalPlayer.Character.HumanoidRootPart,
        TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear),
        {CFrame = P}
    ):Play()
end

function click()
    local VirtualUser = game:GetService('VirtualUser')
    VirtualUser:CaptureController()
    VirtualUser:ClickButton1(Vector2.new(50, 50), CFrame.new(Vector3.new(0, 0, 0)))
end







Black_list = {}

PLY = {}


spawn(function()
    while true do
        wait(100)
        table.clear(PLY)
        for i, v in pairs(game:GetService("Players"):GetChildren()) do
            if v.Team and v.Team.Name == "Pirates" and v.Name ~= game.Players.LocalPlayer.Name then
                table.insert(PLY, v.Name)
            end
        end
    end
end)





spawn(function()
    while wait() do
        pcall(function()
            if Kaitun_FirstSea then
                local level = game.Players.LocalPlayer.Data.Level.Value
                if level == 1 or level <= 15 then
                    Auto_Farm_LV = true
                elseif level == 16 or level <= 60 then
                    Auto_Farm_LV = false
                    Auto_Fast_Shanda = true
                elseif level == 61 or level <= 200 then
                    if string.find(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("PlayerHunter"), "I don't have anything") then
                        Auto_Farm_LV = true
                        Auto_Fast_Shanda = false
                        Auto_Fast_Player = false
                    else
                        Name_Hunter = game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text:match("Defeat%s+(.-)%s+%(")
                        if math.abs(game.Players.LocalPlayer.Data.Level.Value - game.Players[Name_Hunter].Data.Level.Value) == 50 or math.abs(game.Players.LocalPlayer.Data.Level.Value - game.Players[Name_Hunter].Data.Level.Value) <= 110 then
                            Auto_Fast_Player = true
                            Auto_Farm_LV = false
                            Auto_Fast_Shanda = false
                        else
                            print("1")
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
                            if not table.find(Black_list, Name_Hunter) then
                                table.insert(Black_list, Name_Hunter)
                            end
                            if #Black_list == #PLY then
                                print("3")
                                Auto_Farm_LV = true
                                Auto_Fast_Shanda = false
                                Auto_Fast_Player = false
                            end
                        end
                    end
                end
            end
        end)
    end
end)



















--- Player Hunter
spawn(function()
    while wait() do
        if Auto_Fast_Player and game.Players.LocalPlayer.Character.Humanoid.Health  > 0 then
            local quest_title = game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text
            Name_Hunter = game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text:match("Defeat%s+(.-)%s+%(")
            if string.find(quest_title, "Defeat") and string.find(quest_title, "(0/1)") then
                for i,v in pairs(game:GetService("Workspace").Characters:GetChildren()) do
                    if v.Name == tostring(Name_Hunter) and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 and v.Parent then
                        if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - v.HumanoidRootPart.Position).Magnitude <= 170 or (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 170 then
                            starttime = os.time()
                            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame
                            repeat wait()
                                if not game.Players.LocalPlayer.Character:FindFirstChild('HasBuso') then
                                    game.ReplicatedStorage.Remotes.CommF_:InvokeServer('Buso')
                                end
                                if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.PvpDisabled.Visible == false then
                                    v.HumanoidRootPart.Size = Vector3.new(80,80,80)
                                    TP(v.HumanoidRootPart.CFrame * CFrame.new(0, 0, 5))
                                    if game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Character:FindFirstChild("Black Leg").Level.Value >= 150 then
                                        game:service('VirtualInputManager'):SendKeyEvent(true, "V", false, game)
                                        game:service('VirtualInputManager'):SendKeyEvent(false, "V", false, game)
                                    end
                                    click()
                                    game:service('VirtualInputManager'):SendKeyEvent(true, "X", false, game)
                                    game:service('VirtualInputManager'):SendKeyEvent(false, "X", false, game)
                                    wait(.1)
                                    if starttime - os.time() > 60 then
                                        print("2")
                                        table.insert(Black_list, Name_Hunter)
                                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
                                    end
                                else
                                    repeat wait() game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EnablePvp") until game:GetService("Players")["LocalPlayer"].PlayerGui.Main.PvpDisabled.Visible == false
                                end
                            until not Auto_Fast_Player or v.Humanoid.Health <= 0 or not v.Parent or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false or not Kaitun_FirstSea
                        
                        else
                            TP(v.HumanoidRootPart.CFrame)
                        end
                    end
                end
            end
        end
    end
end)








--- Auto Shanda
spawn(function()
    while wait() do
        pcall(function()
        if Auto_Fast_Shanda and  game.Players.LocalPlayer.Character.Humanoid.Health  > 0 then   
                local Shand_pos = CFrame.new(-7685.666015625, 5567.17724609375, -501.0447998046875)
                if game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false then
                        if game:GetService("Workspace").Enemies:FindFirstChild("Shanda") then
                            if game:GetService("Workspace").Enemies:FindFirstChild("Shanda") then
                                for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                                    if v:FindFirstChild('Humanoid')  and  v:FindFirstChild('HumanoidRootPart') and v.Name == "Shanda" then
                                        repeat wait()
                                            if not game.Players.LocalPlayer.Character:FindFirstChild('HasBuso') then
                                                game.ReplicatedStorage.Remotes.CommF_:InvokeServer('Buso')
                                            end
                                            StartMagnet_Fast = true
                                            TP(v.HumanoidRootPart.CFrame * CFrame.new(0,30,0))
                                            v.HumanoidRootPart.Size = Vector3.new(60,60,60)
                                            v.HumanoidRootPart.Transparency = 1
                                            v.Humanoid.JumpPower = 0
                                            v.Humanoid.WalkSpeed = 0
                                            v.HumanoidRootPart.CanCollide = false
                                            v.Humanoid:ChangeState(11)
                                            v.Humanoid:ChangeState(14)
                                            Pos_Mon = v.HumanoidRootPart.CFrame
                                            click()
                                            until  v.Humanoid.Health <= 0 or not v.Parent  or not Auto_Fast_Shanda or game.Players.LocalPlayer.Data.Level.Value > 60
                                            StartMagnet_Fast = false
                                    end
                                end
                            end
                        elseif not game:GetService("Workspace").Enemies:FindFirstChild("Shanda") then
                            if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Shand_pos.Position).magnitude > 3000 then
                                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-7894.6176757813, 5547.1416015625, -380.29119873047))
                            else
                                TP(Shand_pos)
                            end
                        end
                else
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
                end
            end
        end)
    end
end)






----- Auto Farm LV
spawn(function()
    while wait() do
        if  Auto_Farm_LV  and  game.Players.LocalPlayer.Character.Humanoid.Health  > 0 then
            pcall(function()
                if game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false then
                    checklv()
                    repeat wait()
                        local distance_quest = (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - POSQuest.Position).magnitude
                        if distance_quest <= 5 then
                            wait(.5)
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest",NameQ,Lvq)
                        else
                            TP(POSQuest)
                        end
                    until   game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true or not Kaitun_FirstSea or not Auto_Farm_LV
                elseif game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true then
                    checklv()
                    if not string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text,NameMon) then
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
                    end
                    if game:GetService("Workspace").Enemies:FindFirstChild(NameMon) then
                        for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                            if v:FindFirstChild('Humanoid')  and  v:FindFirstChild('HumanoidRootPart') then
                                if v.Name == NameMon then
                                    repeat wait()
                                            if not game.Players.LocalPlayer.Character:FindFirstChild('HasBuso') then
                                                game.ReplicatedStorage.Remotes.CommF_:InvokeServer('Buso')
                                            end
                                            StartMagnet = true
                                            TP(v.HumanoidRootPart.CFrame * CFrame.new(0,30,0))
                                            v.HumanoidRootPart.Size = Vector3.new(60,60,60)
                                            v.HumanoidRootPart.Transparency = 1
                                            v.Humanoid.JumpPower = 0
                                            v.Humanoid.WalkSpeed = 0
                                            v.HumanoidRootPart.CanCollide = false
                                            v.Humanoid:ChangeState(11)
                                            v.Humanoid:ChangeState(14)
                                            Pos_Mon = v.HumanoidRootPart.CFrame
                                            click()
                                    until  v.Humanoid.Health <= 0 or not v.Parent or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false or not Kaitun_FirstSea or not Auto_Farm_LV
                                    StartMagnet = false
                                end
                            end
                        end
                    elseif not game:GetService("Workspace").Enemies:FindFirstChild(NameMon) then
                        TP(POSMON)
                    end
                end
            end)
        end
    end
end)






----- Bring Mon Shanda
spawn(function()
    game:GetService("RunService").Heartbeat:Connect(function()
        pcall(function()
            for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                if  Auto_Fast_Shanda and StartMagnet_Fast and v.Name == "Shanda" and (v.HumanoidRootPart.Position - Pos_Mon.Position).Magnitude <= 260 then
                    v.HumanoidRootPart.CFrame = Pos_Mon
                    v.HumanoidRootPart.CanCollide = false
                    v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                    if v.Humanoid:FindFirstChild("Animator") then
                        v.Humanoid.Animator:Destroy()
                    end
                    sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius",  math.huge)
                end
            end
        end)
    end)
end)




--- Bring Mon AutoFram Lv
spawn(function()
    game:GetService("RunService").Heartbeat:Connect(function() checklv()
        pcall(function()
            for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                if Auto_Farm_LV  and StartMagnet and v.Name == NameMon and (v.HumanoidRootPart.Position - Pos_Mon.Position).Magnitude <= 250 then
                    v.HumanoidRootPart.CFrame = Pos_Mon
                    v.HumanoidRootPart.CanCollide = false
                    v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                    if v.Humanoid:FindFirstChild("Animator") then
                        v.Humanoid.Animator:Destroy()
                    end
                    sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius",  math.huge)
                end
            end
        end)
    end)
end)










                --     local ply = game.Players:GetPlayers()
                --     ------------------------------------   If Player have only me or Playerhunter Quest Can  not do  --------------------------------------
                --     if string.find(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("PlayerHunter"), "I don't have anything") or (ply-1) == 0  then

                --     else
                --         local = quest_title = game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text
                --         if string.find(quest_title, "Defeat") and string.find(quest_title, "(0/1)") then
                --             Name_Hunter = quest_title:match("Defeat%s+(.-)%s+%(")
                --             if (math.abs(game.Players.LocalPlayer.Data.Level.Value - game.Players[Name_Hunter].Data.Level.Value) == 50 or math.abs(game.Players.LocalPlayer.Data.Level.Value - game.Players[Name_Hunter].Data.Level.Value) <= 105) and game:GetService("Players")[Name_Hunter].PlayerGui.Main.PvpDisabled.Visible == false then
                --                 if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.PvpDisabled.Visible == false then
                --                     for i,v in pairs(game:GetService("Workspace").Characters:GetChildren()) do
                --                         if v.Name == Name_Hunter then
                --                             if v:FindFirstChild('Humanoid') and v:FindFirstChild("HumanoidRootPart") then
                --                                 repeat wait()
                --                                     TP(v.HumanoidRootPart.CFrame * CFrame.new(0,0,5))
                --                                     v.HumanoidRootPart.Size = Vector3.new(60,60,60)
                --                                     v.HumanoidRootPart.Transparency = 1
                --                                     v.Humanoid.JumpPower = 0
                --                                     v.Humanoid.WalkSpeed = 0
                --                                     v.HumanoidRootPart.CanCollide = false
                --                                     v.Humanoid:ChangeState(11)
                --                                     v.Humanoid:ChangeState(14)
                --                                     click()
                --                                     if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - v.HumanoidRootPart.position).magnitude <= 15
                --                                         game:service('VirtualInputManager'):SendKeyEvent(true, "Z", false, game)
                --                                         wait(.1)
                --                                         game:service('VirtualInputManager'):SendKeyEvent(false, "Z", false, game)
                --                                         wait(3)
                --                                         game:service('VirtualInputManager'):SendKeyEvent(true, "X", false, game)
                --                                         wait(.1)
                --                                         game:service('VirtualInputManager'):SendKeyEvent(false, "X", false, game)
                --                                     end
                --                                 until  not Kaitun_FirstSea or v.Humanoid.Health <= 0 or not v.Parent or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false
                --                             end
                --                         end
                --                     end
                --                 else
                --                     repeat wait(.1) game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EnablePvp") until game:GetService("Players")["LocalPlayer"].PlayerGui.Main.PvpDisabled.Visible == false
                --                 end
                --             else
                --                 table.insert(Blacklist_ply,Name_Hunter)
                --                 game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
                --                 if #Blacklist_ply == (ply-1) and next(Player_huster_list) != nil then
                --                     if  game.Players.LocalPlayer.Character.Humanoid.Health  > 0 then
                --                         if game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false then
                --                             checklv()
                --                             repeat wait()
                --                                 local distance_quest = (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - POSQuest.Position).magnitude
                --                                 if distance_quest <= 5 then
                --                                     wait(.5)
                --                                     game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest",NameQ,Lvq)
                --                                 else
                --                                     TP(POSQuest)
                --                                 end
                --                             until   game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true or not Kaitun_FirstSea
                --                     elseif game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == true then
                --                             checklv()
                --                             if not string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text,NameMon) then
                --                                 game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
                --                             end
                --                             if game:GetService("Workspace").Enemies:FindFirstChild(NameMon) then
                --                                 for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                --                                     if v:FindFirstChild('Humanoid')  and  v:FindFirstChild('HumanoidRootPart') then
                --                                         if v.Name == NameMon then
                --                                             repeat wait()
                --                                                     if not game.Players.LocalPlayer.Character:FindFirstChild('HasBuso') then
                --                                                         game.ReplicatedStorage.Remotes.CommF_:InvokeServer('Buso')
                --                                                     end
                --                                                     StartMagnet = true
                --                                                     TP(v.HumanoidRootPart.CFrame * CFrame.new(0,30,0))
                --                                                     v.HumanoidRootPart.Size = Vector3.new(60,60,60)
                --                                                     v.HumanoidRootPart.Transparency = 1
                --                                                     v.Humanoid.JumpPower = 0
                --                                                     v.Humanoid.WalkSpeed = 0
                --                                                     v.HumanoidRootPart.CanCollide = false
                --                                                     v.Humanoid:ChangeState(11)
                --                                                     v.Humanoid:ChangeState(14)
                --                                                     Pos_Mon = v.HumanoidRootPart.CFrame
                --                                                     click()
                --                                             until  v.Humanoid.Health <= 0 or not v.Parent or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false or not Kaitun_FirstSea
                --                                             StartMagnet = false
                --                                         end
                --                                     end
                --                                 end
                --                 end
                --             end
                --         end        
                --     end
                -- end







--TP

















































--- Fast Attack
local CameraShaker = require(game.ReplicatedStorage.Util.CameraShaker)
for i,v in pairs(getreg()) do
    if typeof(v) == "function" and getfenv(v).script == game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework then
        for x,w in pairs(debug.getupvalues(v)) do
             if typeof(w) == "table" then
                spawn(function()
                    game:GetService("RunService").RenderStepped:Connect(function()
                        if Auto_Fast_Shanda or Auto_Farm_LV then
                            pcall(function()
                                if game.Players.LocalPlayer.Character:FindFirstChild("Combat") or game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") or game.Players.LocalPlayer.Character:FindFirstChild("Electro") or game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate") or game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw") or game.Players.LocalPlayer.Character:FindFirstChild("Superhuman") or game.Players.LocalPlayer.Character:FindFirstChild("Sharkman Karate") then
                                    w.activeController.increment = 3
                                else
                                    w.activeController.increment = 4
                                end
                                CameraShaker:Stop()
                                w.activeController.timeToNextAttack = -(math.huge^math.huge^math.huge)
                                w.activeController.attacking = false
                                w.activeController.timeToNextBlock = 0
                                w.activeController.blocking = false                            
                                w.activeController.hitboxMagnitude = 50
                                w.activeController.humanoid.AutoRotate = true
                                w.activeController.focusStart = 0
                            end)
                        end
                    end)
                end)
            end
        end
    end
end








--- Auto Stas
spawn(function()
    while true do wait(.3)
        local stast_Melee = tonumber(game.Players.LocalPlayer.Data.Stats.Melee.Level.Value)
        local stast_Defense = tonumber(game.Players.LocalPlayer.Data.Stats.Defense.Level.Value)
        local distance_ = stast_Melee - stast_Defense
        if tonumber(game.Players.LocalPlayer.Data.Stats.Melee.Level.Value) < 1300   then
            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", "Melee", "10")
        elseif tonumber(game.Players.LocalPlayer.Data.Stats.Defense.Level.Value) < 1300 and tonumber(game.Players.LocalPlayer.Data.Stats.Melee.Level.Value) >= 1300   then
            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", "Defense", "10")
        end
    end
end)

function Equip(Itme)
    if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild(Itme) then
       wait(.1)
       game.Players.LocalPlayer.Character.Humanoid:EquipTool(game:GetService("Players").LocalPlayer.Backpack:FindFirstChild(Itme))
    end
end




spawn(function()
    while game.Players.LocalPlayer.Character.Humanoid.Health > 0  do wait(.3)
        pcall(function()
            if (game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectro") == 0 ) and (game.Players.LocalPlayer.Backpack:FindFirstChild("Combat") or game:GetService("Workspace").Characters[game.Players.LocalPlayer.Name]:FindFirstChild("Combat")) then
                if game.Players.LocalPlayer.Data.Beli.Value >= 500000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectro")
                else 
                    repeat wait(.1)
                        Equip("Combat")
                    until not Kaitun_FirstSea or  game.Players.LocalPlayer.Data.Beli.Value >= 500000
                end
            end
        end)
    end
end)





-- Blacklist_ply = {}
-- spawn(function()
--     while wait() do
--         if Check_everthing  and game.Players.LocalPlayer.Character.Humanoid.Health  > 0   then
--             pcall(function()
--             end)
--         end
--     end
-- end)




-- Check Player hunter
-- Player_huster_list = {}
-- spawn(function()
--     while wait(.1) do
--         if check_ply_hunter  and not Kaitun_FirstSea and not Auto_Fast_1  and game.Players.LocalPlayer.Character.Humanoid.Health  > 0   then
--             pcall(function()
--                 if not  string.find(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("PlayerHunter"), "I don't have anything") then
--                     local quest_title = game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text
--                     if game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false then
--                         game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("PlayerHunter")
--                     elseif  game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible ==  true and string.find(quest_title, "Defeat") and string.find(quest_title, "(0/1)") then
--                         name = quest_title:match("Defeat%s+(.-)%s+%(")
--                         local distance_LV = math.abs(game.Players.LocalPlayer.Data.Level.Value - game.Players[name].Data.Level.Value)
--                         if distance_LV == 50 or distance_LV <= 103 then
--                             if game:GetService("Workspace").Characters:FindFirstChild(name) then
--                                 for i,v in pairs(game:GetService("Workspace").Characters:GetChildren()) do
--                                     if v.Name == name then 
--                                         if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") then
--                                             if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.PvpDisabled.Visible == false and game:GetService("Players")[name].PlayerGui.Main.PvpDisabled.Visible == false then
--                                                 repeat wait()
--                                                     TP(v.HumanoidRootPart.CFrame * CFrame.new(0,0,5))
--                                                     v.HumanoidRootPart.Size = Vector3.new(60,60,60)
--                                                     v.HumanoidRootPart.Transparency = 1
--                                                     v.Humanoid.JumpPower = 0
--                                                     v.Humanoid.WalkSpeed = 0
--                                                     v.HumanoidRootPart.CanCollide = false
--                                                     v.Humanoid:ChangeState(11)
--                                                     v.Humanoid:ChangeState(14)
--                                                     click()
--                                                     if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - v.HumanoidRootPart.position).magnitude <= 15
--                                                         game:service('VirtualInputManager'):SendKeyEvent(true, "Z", false, game)
--                                                         wait(.1)
--                                                         game:service('VirtualInputManager'):SendKeyEvent(false, "Z", false, game)
--                                                         wait(3)
--                                                         game:service('VirtualInputManager'):SendKeyEvent(true, "X", false, game)
--                                                         wait(.1)
--                                                         game:service('VirtualInputManager'):SendKeyEvent(false, "X", false, game)
--                                                     end
--                                                     until not check_ply_hunter or  v.Humanoid.Health <= 0 or not v.Parent or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false or not Kaitun_FirstSea
--                                             elseif game:GetService("Players")["LocalPlayer"].PlayerGui.Main.PvpDisabled.Visible == true and game:GetService("Players")[name].PlayerGui.Main.PvpDisabled.Visible == false  then
--                                                 game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EnablePvp")
--                                             elseif game:GetService("Players")["LocalPlayer"].PlayerGui.Main.PvpDisabled.Visible == false and game:GetService("Players")[name].PlayerGui.Main.PvpDisabled.Visible == true  then
--                                                 game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
--                                                 table.insert(Player_huster_list,name)
--                                             end
--                                         end
--                                     end
--                                 end
--                             end
--                         else
--                             game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
--                             local ply = game.Players:GetPlayers()
--                             if next(Player_huster_list) == nil then
--                                 table.insert(Player_huster_list,name)
--                             elseif #Player_huster_list == (#ply-1) then
--                                 check_ply_hunter = false
--                                 Kaitun_FirstSea = true
--                             end
--                         end
--                     end
--                 else
--                     Kaitun_FirstSea = true
--                 end
--             end)
--         end
--     end
-- end)




-- Noclip
spawn(function()
    pcall(function()
        game:GetService("RunService").Stepped:Connect(function()
            if Auto_Fast_Shanda or Auto_Farm_LV or Auto_Fast_Player  then
                if not game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip") then
                    local Noclip = Instance.new("BodyVelocity")
                    Noclip.Name = "BodyClip"
                    Noclip.Parent = game.Players.LocalPlayer.Character.HumanoidRootPart
                    Noclip.MaxForce = Vector3.new(100000,100000,100000)
                    Noclip.Velocity = Vector3.new(0,0,0)
                end
            else	
                if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip") then
                    game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip"):Destroy()
                end
            end
        end)
    end)
end)

spawn(function()
    pcall(function()
        game:GetService("RunService").Stepped:Connect(function()
            if Auto_Fast_Shanda or Auto_Farm_LV or Auto_Fast_Player then
                for _, v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
                    if v:IsA("BasePart") then
                        v.CanCollide = false
                    end
                end
            end
        end)
    end)
end)
