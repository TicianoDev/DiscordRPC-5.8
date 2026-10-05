# Discord RPC for Unreal Engine 5.8

A fully functional Discord Rich Presence plugin updated and tested for **Unreal Engine 5.8**.

Fork From [LouisRaverdy](https://github.com/LouisRaverdy/DiscordRPC)

---

## Installation

1. Download or clone this repository.
2. Copy the entire `DiscordRpc` folder into your Unreal Engine installation's Plugins directory:

```
C:\Program Files\Epic Games\UE_5.8\Engine\Plugins\
```

(Or the equivalent path if you installed Unreal in a different location)

Final structure should look like this:

```
UE_5.8/
└── Engine/
    └── Plugins/
        └── DiscordRpc/
            ├── DiscordRpc.uplugin
            ├── Source/
            └── ...
```

3. Restart the Unreal Editor (or open it if it was closed).
4. Go to **Edit → Plugins**, search for **Discord RPC** and enable it.
5. Restart the editor when prompted.

The plugin will now be available in all your Unreal Engine 5.8 projects.

---

## Initialization

In order to establish a connection with the application you have created before and the discord app 
You need to create something like this in your **Game Instance**  : 

![InitDiscord](https://user-images.githubusercontent.com/47295080/147773538-c4ac76cd-2199-4a1a-af90-cc695d8c0386.png)

> **Note :** Make sure your Game Instance is defined as default in the Project Settings. (Project Settings -> Maps & Modes -> Game Instance Class)

For remove your presence when you exit the game you need to add this to your **Game Instance** :

![shutdown](https://user-images.githubusercontent.com/47295080/192113957-b7675e3f-161d-4d23-bb98-e5ce6f48a586.png)

## Nodes 

To update your presence for your game, you can use this code (read the image next to it to understand the fields of the node) : 

![SetPresenceDiscord](https://user-images.githubusercontent.com/47295080/147773549-6f106fda-835d-4cff-97f8-c220627b2dbf.png)

> **Note :** To use image in rich presence you need to upload them on your Discord developer game page (Rich Presence -> Art Assets)
