# Library-script-v2

## loadstring script web
```lua
loadstring(game:HttpGet(('-- link'),true))()
```

# copiar algo para a área e transferência
```lua
setclipboard("-- msg")
```

## depois e um tempo vai executar algo
```lua
wait(3) -- em segundos
```

## criar notificações
```lua
game.StarterGui:SetCore("SendNotification", {
    Title = "título";
    Text = "descrição";
})
```


## criar notificações diferentes
```lua
local Notif = Instance.new("ScreenGui") 
local TextLabel = Instance.new("TextLabel") 

Notif.Name = "Notification" 
Notif.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui") 

TextLabel.Parent = Notif 
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255) 
TextLabel.Size = UDim2.new(1, 0, 1, 0) 
TextLabel.Text = "This is a notification!" 
TextLabel.TextColor3 = Color3.fromRGB(0, 0, 0) 
TextLabel.TextScaled = true 

wait(2) -- em segundos
Notif:Destroy()
```


## script e resetar o personagem
```lua
game.Players.LocalPlayer.Character.Humanoid.Health = 0
```

## mude o número da saúde o player
```lua
local jogador = game.Players.LocalPlayer

jogador.Character.Humanoid.Health = 50
```

## script e kick
```lua
game.Players.LocalPlayer:Kick("kick")
```


## aumentar velocidade (padrão: 16)
```lua
local humanoid = game.Players.LocalPlayer.Character.Humanoid
humanoid.WalkSpeed = 50 -- speed
```

## aumentar pulo (padrão: 50)
```lua
local player = game.Players.LocalPlayer
local character = player.Character

local jumpHeight = 50

local humanoid = character:WaitForChild("Humanoid")

humanoid.JumpPower = jumpHeight
```

## mudar pov (padrão: 70)
```lua
game.Workspace.CurrentCamera.FieldOfView = 70
```

## chat local
```lua
local args = {
    [1] = "oi",
    [2] = "All"
}

game:GetService("ReplicatedStorage"):WaitForChild("DefaultChatSystemChatEvents"):WaitForChild("SayMessageRequest"):FireServer(unpack(args))
```

## teleporte
```lua
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-- posição)
```

## rejoin
```lua
wait(1)	
game:GetService("TeleportService"):Teleport(game.PlaceId, game.Players.LocalPlayer)
```


