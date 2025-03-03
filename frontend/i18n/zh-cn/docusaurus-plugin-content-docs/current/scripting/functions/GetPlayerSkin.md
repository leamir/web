---
title: GetPlayerSkin
sidebar_label: GetPlayerSkin
description: Returns the class of the players skin.
tags: ["player"]
---

## Description

Returns the class of the players skin

| Name     | Description                              |
| -------- | ---------------------------------------- |
| playerid | The player you want to get the skin from |

## Returns

The [skin id](../resources/skins).

**0** if invalid.

## Examples

```c
public OnPlayerCommandText(playerid, cmdtext[])
{
    if (!strcmp(cmdtext, "/myskin", true))
    {
        new string[32];
        new playerSkin = GetPlayerSkin(playerid);

        format(string, sizeof(string), "Your skin id: %d", playerSkin);
        SendClientMessage(playerid, -1, string);
        return 1;
    }
    return 0;
}
```

## Notes

:::tip

Returns the new skin after [SetSpawnInfo](SetSpawnInfo) is called but before the player actually respawns to get the new skin. Returns the old skin if the player was spawned through [SpawnPlayer](SpawnPlayer) function.

:::

## Related Functions

- [SetPlayerSkin](SetPlayerSkin): Set a player's skin.

## Related Resources

- [Skin IDs](../resources/skins)
