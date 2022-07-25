
<p>
  <img src="https://i.imgur.com/yD5kN0y.png" />    
</p>


Usage
```csharp
Window(<string> title)
   Toggle(<string> text, <function> callback)
   Slider(<string> text, <table> options {max, default}, <function> callback)
```
  
Example
```lua
local lib = loadstring(game:HttpGet('https://raw.githubusercontent.com/0xd5f/ui-lib/main/main.lua'))()
local window = lib:Window('title here')

window:Toggle('toggle', function(enabled)
     print(enabled)
end)

window:Slider('slider', {
     max = 80,
     def = 20
}, function(value)
     print(value)
end)
```
