# minecraft-world

My singleplayer minecraft world, thought it would be kind of cool to save this to Github so I never lose it and can branch / fork if stuff goes really wrong lol

# Fish scripts for saving and loading

```
function mcsave
   cd ~/.minecraft/saves/minecraft-world
   git add .
   git commit -m "$argv"
   git push
   cd -
end

function mcload
   cd ~/.minecraft/saves/minecraft-world
   git pull
   cd -
end
```
