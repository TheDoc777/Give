**Give** limits item giving by only allowing players with the relevant permissions access to give items *(by item ID or item name, when available)* to themselves or other players. *By default*, this will override and replace any commands that share the same name.

## Dependencies

### Optional

- [Kits](https://umod.org/plugins/kits)

If the Kits plugin is installed, players can also give kits if they have the permission.

## Permissions

- `give.self` -- Allows giving item(s) to self
- `give.all` -- Allows giving item(s) to ***all*** players
- `give.to` -- Allows giving item(s) to other players
- `give.arm` -- Allows giving item(s) to player's belt ***(Reign of Kings and Rust only)***
- `give.kit` -- Allows giving kit(s) to players ***(Kits plugin must be installed and loaded)***

## Commands

This plugin provides universal chat and console commands. When using a command in the chat, prefix it with a forward slash: `/`.

- `give <item id or item name> [amount] [player name or id]` -- Give an item to self or another player
- `givekit <kit name> [player name or id]` -- Give an available kit to self or another player

## Configuration

```json
{
  "Item blacklist (name or item ID)": [
    "rock",
    "torch"
  ],
  "Log usage to console (true/false)": false,
  "Show chat notices (true/false)": true,
  "Show popup notices (true/false)": true
}
```

## Localization

The default messages are in the `Give.json` file under the `oxide/lang/en` directory. To add support for another language, create a new language folder (ex. de for German) if not already created, copy the default language file to the new folder, and then customize the messages.
