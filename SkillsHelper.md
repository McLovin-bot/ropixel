# SkillsHelper
## The Basics
### Example of each function (Add xp, Render Skills)
``` Lua
-- Getting module from ServerScriptService

local skillsHelper = require(game:GetService("ServerScriptService"):WaitForChild("SkillsHelper"))

-- Initilize the module
-- We are pretty much storing the player object 
local skills = skillsHelper.new(p)

-- Add xp (skill name, amount)
-- Example adding 10 foraging xp

skills:addXp("Foraging", 10)

-- Render Skills

skills:renderSkills()
```

<hr>

# Methods

<hr>

## skills:`addXp`
``` Lua
skills:addXp(Skill Name, Amount)
```
> Amount = number

> Skill Name = String

> This function takes two parameters Amount of xp and the name of the skill
> 
<hr>

## skills:`renderSkills`
``` Lua
skills:renderSkills()
```
> this function takes no parameters

> used to update skills gui

<hr>

## skills.`new`
``` Lua
skills.new(player)
```
> function takes one parameter of a player object

> player = player object

> We are pretty much storing the player object 

> this sets up the skills var as a skillsHelper object

> Reason:

> instead of having to do skills:addXp(player, skill, amount)
> we can do skills:addXp(skill, amount)

> we don't have to pass the player object because we save it when we use the .new method







