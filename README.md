# Arena Game

Create a new game process

```
.load arena.lua

.load ao-effect.lua

.load-blueprint token

PaymentToken = ao.id
```

# Create a player

```
.load ao-effect-bot.lua

Game = "game_process_id"

Send({ Target = Game, Action = "RequestTokens" })

Send({ Target = Game, Action = "Register" })

```

Then send tick from game

```
Send({ Target = ao.id, Action = "Tick" })
```
