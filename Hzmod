local Players = game:GetService("Players")

local player = Players.LocalPlayer

local playerGui = player:FindFirstChild("PlayerGui") or player:WaitForChild("PlayerGui")

 

-- Tạo Menu thông báo đề mô đầu tiên

local ScreenGui = Instance.new("ScreenGui")

ScreenGui.Name = "HzmodDemoNotice"

ScreenGui.ResetOnSpawn = false

ScreenGui.Parent = playerGui

 

local MainFrame = Instance.new("Frame")

MainFrame.Size = UDim2.new(0, 320, 0, 160)

MainFrame.Position = UDim2.new(0.5, -160, 0.5, -80)

MainFrame.BackgroundColor3 = Color3.fromRGB(30, 30, 30)

MainFrame.BorderSizePixel = 0

MainFrame.Parent = ScreenGui

 

local UICorner = Instance.new("UICorner")

UICorner.CornerRadius = UDim.new(0, 8)

UICorner.Parent = MainFrame

 

local Title = Instance.new("TextLabel")

Title.Size = UDim2.new(1, 0, 0, 40)

Title.Position = UDim2.new(0, 0, 0, 10)

Title.BackgroundTransparency = 1

Title.Text = "⚠️ THÔNG BÁO DEMO"

Title.TextColor3 = Color3.fromRGB(255, 255, 255)

Title.TextSize = 18

Title.Font = Enum.Font.GothamBold

Title.Parent = MainFrame

 

local Content = Instance.new("TextLabel")

Content.Size = UDim2.new(1, -20, 0, 50)

Content.Position = UDim2.new(0, 10, 0, 50)

Content.BackgroundTransparency = 1

Content.Text = "Đây là bản đề mô thôi, ít chức năng nên thông cảm nha"

Content.TextColor3 = Color3.fromRGB(200, 200, 200)

Content.TextSize = 14

Content.Font = Enum.Font.Gotham

Content.TextWrapped = true

Content.Parent = MainFrame

 

local Button = Instance.new("TextButton")

Button.Size = UDim2.new(0, 100, 0, 35)

Button.Position = UDim2.new(0.5, -50, 1, -45)

Button.BackgroundColor3 = Color3.fromRGB(0, 120, 215)

Button.BorderSizePixel = 0

Button.Text = "OK"

Button.TextColor3 = Color3.fromRGB(255, 255, 255)

Button.TextSize = 16

Button.Font = Enum.Font.GothamBold

Button.Parent = MainFrame

 

local ButtonCorner = Instance.new("UICorner")

ButtonCorner.CornerRadius = UDim.new(0, 6)

ButtonCorner.Parent = Button

 

-- Khi bấm OK ở bảng 1 sẽ hiện tiếp bảng thứ 2

Button.MouseButton1Click:Connect(function()

    ScreenGui:Destroy()

    

    -- Tạo bảng thông báo thứ 2 (Bản quyền / Cre)

    local SecondGui = Instance.new("ScreenGui")

    SecondGui.Name = "DarkHubCreditNotice"

    SecondGui.ResetOnSpawn = false

    SecondGui.Parent = playerGui

 

    local SecondFrame = Instance.new("Frame")

    SecondFrame.Size = UDim2.new(0, 340, 0, 180)

    SecondFrame.Position = UDim2.new(0.5, -170, 0.5, -90)

    SecondFrame.BackgroundColor3 = Color3.fromRGB(30, 30, 30)

    SecondFrame.BorderSizePixel = 0

    SecondFrame.Parent = SecondGui

 

    local SecondCorner = Instance.new("UICorner")

    SecondCorner.CornerRadius = UDim.new(0, 8)

    SecondCorner.Parent = SecondFrame

 

    local SecondTitle = Instance.new("TextLabel")

    SecondTitle.Size = UDim2.new(1, 0, 0, 40)

    SecondTitle.Position = UDim2.new(0, 0, 0, 10)

    SecondTitle.BackgroundTransparency = 1

    SecondTitle.Text = "???? THÔNG TIN SCRIPT"

    SecondTitle.TextColor3 = Color3.fromRGB(255, 255, 0)

    SecondTitle.TextSize = 18

    SecondTitle.Font = Enum.Font.GothamBold

    SecondTitle.Parent = SecondFrame

 

    local SecondContent = Instance.new("TextLabel")

    SecondContent.Size = UDim2.new(1, -20, 0, 70)

    SecondContent.Position = UDim2.new(0, 10, 0, 50)

    SecondContent.BackgroundTransparency = 1

    SecondContent.Text = "Script by darkhub\nNếu đăng video thì thêm cre nhé\nTiktok @darkhubvn"

    SecondContent.TextColor3 = Color3.fromRGB(220, 220, 220)

    SecondContent.TextSize = 14

    SecondContent.Font = Enum.Font.Gotham

    SecondContent.TextWrapped = true

    SecondContent.Parent = SecondFrame

 

    local SecondButton = Instance.new("TextButton")

    SecondButton.Size = UDim2.new(0, 100, 0, 35)

    SecondButton.Position = UDim2.new(0.5, -50, 1, -45)

    SecondButton.BackgroundColor3 = Color3.fromRGB(0, 120, 215)

    SecondButton.BorderSizePixel = 0

    SecondButton.Text = "TIẾP TỤC"

    SecondButton.TextColor3 = Color3.fromRGB(255, 255, 255)

    SecondButton.TextSize = 16

    SecondButton.Font = Enum.Font.GothamBold

    SecondButton.Parent = SecondFrame

 

    local SecondButtonCorner = Instance.new("UICorner")

    SecondButtonCorner.CornerRadius = UDim.new(0, 6)

    SecondButtonCorner.Parent = SecondButton

 

    -- Khi bấm TIẾP TỤC ở bảng 2 sẽ tắt bảng đó và load menu chính WindUI

    SecondButton.MouseButton1Click:Connect(function()

        SecondGui:Destroy()

        

        -- Load WindUI

        local WindUI = loadstring(game:HttpGet("https://raw.githubusercontent.com/Footagesus/WindUI/main/dist/main.lua"))()

 

        local Window = WindUI:CreateWindow({

            Title = "Hzmod",

            SubTitle = "by darkendvn",

            Theme = "Dark",

            MinimizeKey = Enum.KeyCode.RightShift

        })

 

        local TeleportService = game:GetService("TeleportService")

        local HttpService = game:GetService("HttpService")

        local Players = game:GetService("Players")

        local Workspace = game:GetService("Workspace")

        local Lighting = game:GetService("Lighting")

        local PlaceId = game.PlaceId

 

        local FilePath = "Hzmod_Settings.json"

 

        -- Biến lưu trạng thái

        local Settings = {

            LightningWarning = false,

            AutoCollectLightning = false

        }

 

        local isWarningRunning = false

 

        -- Hàm lưu/tải cấu hình

        local function saveSettings()

            local success = pcall(function()

                local encoded = HttpService:JSONEncode(Settings)

                writefile(FilePath, encoded)

            end)

            if success then

                WindUI:Notify({Title = "Setting", Content = "Đã lưu cài đặt thành công!", Duration = 2})

            end

        end

 

        local function loadSettings()

            pcall(function()

                if isfile(FilePath) then

                    local content = readfile(FilePath)

                    local decoded = HttpService:JSONDecode(content)

                    for k, v in pairs(decoded) do

                        Settings[k] = v

                    end

                end

            end)

        end

        loadSettings()

 

        -- Tạo các Tab

        local MainTab = Window:Tab({ Title = "Main", Icon = "home" })

        local ShopTab = Window:Tab({ Title = "Shop", Icon = "shopping-cart" })

        local HopTab = Window:Tab({ Title = "Server Hop", Icon = "server" })

        local SettingTab = Window:Tab({ Title = "Setting", Icon = "settings" })

        local DevTab = Window:Tab({ Title = "Dev", Icon = "code" })

 

        -- ==================== TAB MAIN ====================

        MainTab:Section({ Title = "Tính năng Sét" })

 

        MainTab:Toggle({

            Title = "Cảnh báo sét",

            Description = "Bật/tắt cảnh báo màn hình",

            Default = Settings.LightningWarning,

            Callback = function(state)

                Settings.LightningWarning = state

            end

        })

 

        MainTab:Toggle({

            Title = "Nhặt trước sét",

            Description = "Tự động TP tới và thu hoạch sét ở vườn của bạn",

            Default = Settings.AutoCollectLightning,

            Callback = function(state)

                Settings.AutoCollectLightning = state

            end

        })

 

        -- ==================== TAB SHOP ====================

        -- Trống

 

        -- ==================== TAB SERVER HOP ====================

        HopTab:Section({ Title = "Quản lý Server" })

 

        local function vipServerHop()

            WindUI:Notify({Title = "Server Hop", Content = "Đang tìm server vắng nhất...", Duration = 2})

            local url = "https://games.roblox.com/v1/games/" .. PlaceId .. "/servers/Public?sortOrder=Asc&limit=100"

            local success, result = pcall(function() return HttpService:JSONDecode(game:HttpGet(url)) end)

 

            if success and result and result.data then

                local targetServer = nil

                for _, server in pairs(result.data) do

                    if server.id ~= game.JobId and server.playing < server.maxPlayers then

                        if server.playing <= 2 then

                            targetServer = server.id

                            break

                        end

                    end

                end

                if not targetServer then

                    for _, server in pairs(result.data) do

                        if server.id ~= game.JobId and server.playing < server.maxPlayers then

                            targetServer = server.id

                            break

                        end

                    end

                end

                if targetServer then

                    WindUI:Notify({Title = "Server Hop", Content = "Đang chuyển đến server vắng...", Duration = 3})

                    TeleportService:TeleportToPlaceInstance(PlaceId, targetServer, Players.LocalPlayer)

                else

                    WindUI:Notify({Title = "Server Hop", Content = "Không tìm thấy server trống!", Duration = 3})

                end

            end

        end

 

        HopTab:Button({

            Title = "Hop VIP Server (Tìm server vắng)",

            Description = "Chuyển đến server ít người nhất",

            Callback = function() vipServerHop() end

        })

 

        -- ==================== TAB SETTING ====================

        SettingTab:Section({ Title = "Cài đặt & Lưu trữ" })

 

        SettingTab:Button({

            Title = "Save cài đặt",

            Description = "Lưu trạng thái các nút hiện tại vào file",

            Callback = function()

                saveSettings()

            end

        })

 

        -- ==================== TAB DEV ====================

        DevTab:Section({ Title = "Thông tin nhà phát triển" })

 

        DevTab:Button({

            Title = "Discord admin",

            Description = "Sao chép đường dẫn Discord vào khay nhớ tạm",

            Callback = function()

                pcall(function()

                    setclipboard("https://discord.gg/kS27eTfx8")

                end)

                WindUI:Notify({Title = "Discord", Content = "Đã copy link Discord admin vào bộ nhớ tạm!", Duration = 3})

            end

        })

 

        -- ==================== HÀM KIỂM TRA VƯỜN CỦA MÌNH ====================

        local function isMyFarm(targetPart)

            local character = player.Character

            if not character or not character:FindFirstChild("HumanoidRootPart") then return false end

            

            local current = targetPart

            while current and current ~= Workspace do

                local parentName = current.Name:lower()

                if parentName:find(player.Name:lower()) then

                    return true

                end

                if current:FindFirstChild("Owner") then

                    local ownerVal = current.Owner.Value

                    if ownerVal == player or (typeof(ownerVal) == "string" and ownerVal:lower() == player.Name:lower()) then

                        return true

                    end

                end

                current = current.Parent

            end

            

            -- Giới hạn khoảng cách (chỉ tính vật thể ở gần nhân vật trong phạm vi 40 studs)

            if targetPart:IsA("BasePart") then

                local distance = (targetPart.Position - character.HumanoidRootPart.Position).Magnitude

                if distance <= 40 then

                    return true

                end

            end

            

            return false

        end

 

        -- ==================== LOGIC NHẶT TRƯỚC SÉT (ĐÃ FIX TP) ====================

        local function checkAndCollectLightning(obj)

            if not Settings.AutoCollectLightning then return end

 

            local name = obj.Name:lower()

            local isLightning = name:find("lightning") or name:find("thunder") or name:find("storm") or name:find("set") or name:find("sét")

            

            if isLightning then

                local targetPart = nil

                if obj:IsA("BasePart") then

                    targetPart = obj

                elseif obj:IsA("Model") then

                    targetPart = obj.PrimaryPart or obj:FindFirstChildWhichIsA("BasePart")

                end

 

                if targetPart and isMyFarm(targetPart) then

                    task.spawn(function()

                        local char = player.Character

                        if char and char:FindFirstChild("HumanoidRootPart") then

                            local hrp = char.HumanoidRootPart

                            -- Dịch chuyển nhân vật ngay lập tức tới sát sét

                            hrp.CFrame = targetPart.CFrame + Vector3.new(0, 3, 0)

                            

                            -- Quét và kích hoạt mọi ProximityPrompt ở gần đó

                            for _, v in pairs(Workspace:GetDescendants()) do

                                if v:IsA("ProximityPrompt") then

                                    local p = v.Parent

                                    if p and (p == targetPart or p.Parent == targetPart or (p:IsA("BasePart") and (p.Position - targetPart.Position).Magnitude < 10)) then

                                        pcall(function()

                                            v.HoldDuration = 0

                                            v.MaxActivationDistance = 9999

                                            fireproximityprompt(v)

                                        end)

                                    end

                                end

                            end

                        end

                    end)

                end

            end

        end

 

        Workspace.DescendantAdded:Connect(function(descendant)

            checkAndCollectLightning(descendant)

        end)

 

        task.spawn(function()

            while true do

                task.wait(0.05)

                if Settings.AutoCollectLightning then

                    pcall(function()

                        for _, v in pairs(Workspace:GetDescendants()) do

                            checkAndCollectLightning(v)

                        end

                    end)

                end

            end

        end)

 

        -- ==================== LOGIC CẢNH BÁO SÉT ====================

        Workspace.DescendantAdded:Connect(function(descendant)

            if Settings.LightningWarning and not isWarningRunning then

                local isHeldByPlayer = false

                local parent = descendant.Parent

                while parent and parent ~= Workspace do

                    if parent:IsA("Model") and Players:GetPlayerFromCharacter(parent) then

                        isHeldByPlayer = true

                        break

                    elseif parent:IsA("Backpack") or parent.Name == "Backpack" then

                        isHeldByPlayer = true

                        break

                    end

                    parent = parent.Parent

                end

                

                if not isHeldByPlayer then

                    local name = descendant.Name:lower()

                    if name:find("plant") or name:find("crop") or name:find("seedling") or name:find("lightning") or name:find("thunder") or name:find("storm") or name:find("set") then

                        

                        isWarningRunning = true

                        

                        task.spawn(function()

                            WindUI:Notify({Title = "⚠️ CẢNH BÁO", Content = "1", Duration = 1})

                            task.wait(1)

                            WindUI:Notify({Title = "⚠️ CẢNH BÁO", Content = "2", Duration = 1})

                            task.wait(1)

                            WindUI:Notify({Title = "⚠️ CẢNH BÁO", Content = "3", Duration = 1})

                            task.wait(1)

                            WindUI:Notify({Title = "⚠️ CẢNH BÁO SÉT!", Content = "Sét", Duration = 2})

                            

                            task.wait(3)

                            isWarningRunning = false

                        end)

                        

                        if descendant:IsA("BasePart") then

                            pcall(function()

                                local h = Instance.new("Highlight", descendant)

                                h.FillColor = Color3.fromRGB(255, 255, 0)

                                task.delay(4, function() h:Destroy() end)

                            end)

                        end

                    end

                end

            end

        end)

 

        WindUI:Notify({Title = "Hzmod Loaded", Content = "Khởi chạy thành công toàn bộ tính năng!", Duration = 3})

    end)

end)
