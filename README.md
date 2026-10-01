# TH Hub

A Trade Hangout hub, built by fruitloop.

![UI preview](image.png)

## Features
- **Spammer:** posts your message in chat on a cooldown, with an optional start delay and anti-AFK.
- **Server Hopper:** moves you to a fuller server when the current one drops below a threshold.
- **Crowd Navigation:** walks your character to where players are gathered.
- **Misc:** AFK status, nametag spam and auto-equipping a held item.
- **Configs:** save, load and delete profiles, auto-load on startup, and copy/paste a config through the clipboard. Settings auto-save to the active profile.

## Install
Run this in your executor:
```lua
loadstring(game:HttpGet("INSERT"))()
```
Profiles are saved in `fruitloop/configs/`, and the hub reloads itself when it hops servers.

### Running from source
Put the 6 `.lua` files in `workspace/fruitloop/` and run `loadstring(readfile("fruitloop/Autospam.lua"))()`.


## Requirements
Your executor must support `getgenv`, `getrawmetatable`/`hookfunction` (for anti-AFK), `readfile`, `writefile`, `isfile`, `makefolder`, `listfiles`, `loadstring` and an HTTP request function. `queue_on_teleport` is needed for server hopping.

The UI uses [Rayfield](https://sirius.menu/rayfield).

## Disclaimer
Using executors breaks Roblox's Terms of Use and can get your account banned. Use this at your own risk.
