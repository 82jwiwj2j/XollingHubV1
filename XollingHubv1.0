-- XollingHub v1.0 - Script básico con menú y opciones farm

local StarterGui = game:GetService("StarterGui")
local Players = game:GetService("Players")
local LocalPlayer = Players.LocalPlayer

-- Crear GUI
local ScreenGui = Instance.new("ScreenGui")
ScreenGui.Name = "XollingHub"
ScreenGui.Parent = LocalPlayer:WaitForChild("PlayerGui")

-- Crear Frame principal
local Frame = Instance.new("Frame")
Frame.Size = UDim2.new(0, 300, 0, 200)
Frame.Position = UDim2.new(0.5, -150, 0.5, -100)
Frame.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
Frame.BorderSizePixel = 0
Frame.Parent = ScreenGui

-- Crear Título
local Title = Instance.new("TextLabel")
Title.Size = UDim2.new(1, 0, 0, 30)
Title.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
Title.TextColor3 = Color3.new(1, 1, 1)
Title.Text = "XollingHub"
Title.Font = Enum.Font.SourceSansBold
Title.TextSize = 20
Title.Parent = Frame

-- Crear ícono (un círculo rojo simple)
local Icon = Instance.new("Frame")
Icon.Size = UDim2.new(0, 25, 0, 25)
Icon.Position = UDim2.new(0, 5, 0, 2)
Icon.BackgroundColor3 = Color3.fromRGB(200, 30, 30)
Icon.BorderSizePixel = 0
Icon.Parent = Title
Icon.ClipsDescendants = true
Icon.AnchorPoint = Vector2.new(0, 0)local IconCircle = Instance.new("UICorner")
IconCircle.CornerRadius = UDim.new(1, 0)
IconCircle.Parent = Icon

-- Crear botón Farm 1
local FarmButton1 = Instance.new("TextButton")
FarmButton1.Size = UDim2.new(0.9, 0, 0, 40)
FarmButton1.Position = UDim2.new(0.05, 0, 0, 40)
FarmButton1.BackgroundColor3 = Color3.fromRGB(70, 70, 70)
FarmButton1.TextColor3 = Color3.new(1, 1, 1)
FarmButton1.Text = "Activar Farm 1"
FarmButton1.Font = Enum.Font.SourceSans
FarmButton1.TextSize = 18
FarmButton1.Parent = Frame-- Crear botón Farm 2
local FarmButton2 = Instance.new("TextButton")
FarmButton2.Size = UDim2.new(0.9, 0, 0, 40)
FarmButton2.Position = UDim2.new(0.05, 0, 0, 90)
FarmButton2.BackgroundColor3 = Color3.fromRGB(70, 70, 70)
FarmButton2.TextColor3 = Color3.new(1, 1, 1)
FarmButton2.Text = "Activar Farm 2"
FarmButton2.Font = Enum.Font.SourceSans
FarmButton2.TextSize = 18
FarmButton2.Parent = Frame

-- Crear botón Cerrar
local CloseButton = Instance.new("TextButton")
CloseButton.Size = UDim2.new(0, 30, 0, 30)
CloseButton.Position = UDim2.new(1, -35, 0, 2)
CloseButton.BackgroundColor3 = Color3.fromRGB(200, 30, 30)
CloseButton.TextColor3 = Color3.new(1, 1, 1)
CloseButton.Text = "X"
CloseButton.Font = Enum.Font.SourceSansBold
CloseButton.TextSize = 20
CloseButton.Parent = Frame- Funciones para farm (ejemplo simple, puedes modificar)

local farm1Active = false
local farm2Active = false

local function farm1()
    while farm1Active do
        -- Aquí iría la lógica real de farm 1
        print("Farm 1 activo...")
        wait(2)
    end
end

local function farm2()
    while farm2Active do
        -- Aquí iría la lógica real de farm 2
        print("Farm 2 activo...")
        wait(3)
    end
end

-- Botón Farm 1 clic
FarmButton1.MouseButton1Click:Connect(function()
    farm1Active = not farm1Active
    if farm1Active then
        FarmButton1.Text = "Detener Farm 1"
        spawn(farm1)
    else
        FarmButton1.Text = "Activar Farm 1"
    end
end)

-- Botón Farm 2 clic
FarmButton2.MouseButton1Click:Connect(function()
    farm2Active = not farm2Active
    if farm2Active then
        FarmButton2.Text = "Detener Farm 2"
        spawn(farm2)
    else
        FarmButton2.Text = "Activar Farm 2"
    end
end)

-- Botón cerrar clic
CloseButton.MouseButton1Click:Connect(function()
    ScreenGui:Destroy()
end)

-- Mensaje de carga
print("XollingHub cargado correctamente")
