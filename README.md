This is a [fork](https://en.wikipedia.org/wiki/Fork_(software_development)) (i.e., a copy with changes) of the QuickSmelt plugin on uMod.

https://umod.org/plugins/quick-smelt

## Differences from uMod/WhiteThunder version

- Smelting/cooking animations are customizable in this version
- Smelting/cooking multiple items at once does not increase efficiency (like vanilla)
- Works with electric furnaces
- Furnaces started via electricity or igniters will function the same as furnaces started directly by a player (uMod version will not detect this, causing furnaces to use vanilla rates in those cases)
- The `OnOvenCook` and `OnOvenCooked` hooks are called correctly, allowing for compatibility with other plugins
- There are two speed options which can be tweaked to achieve your desired smelting speed effect.
- Increasing speed only works using whole numbers, like 2.0, 3.0, 4.0 -- This means you cannot achieve speeds like 0.5 or 1.5
- The "Smelting Frequencies" works. Do not set it to 0, it will cause errors.
- When the plugin loads, if the config has invalid item short names or invalid entity short names, warnings will be printed in the server console to help you learn about the problem as early as possible

## FAQ

#### Why do I get a compilation error?

You may have downloaded the plugin file wrong. Try viewing the cs file in **raw** format (click [here](https://github.com/Feverr92/QuickSmelt/blob/master/QuickSmelt.cs)), then save that as QuickSmelt.cs.

#### Do I need to reset my config to use this fork?

Yes, there are new configuration options.

#### Why is smelting speed having no effect?

There are two speed options in this version. "Items per invocation multiplier" changes how many items in the stack are smelted for each call of the cook command. "Invocations per second" is the frequency the cook command is called. You can edit both of these to achieve your desired smelt speed/ effect.

#### Can I suggest new features?

Nope.

#### How can I speed up industrial conveyors to keep up with the fast smelting speed and high stack sizes?

Try using the Conveyor Stacks plugin and/or adjusting conveyor ConVars.

#### When will this be available on uMod?

I am not currently a uMod contributor.

## Furnace short names

The following prefab short names are valid in the config.

- `bbq.campermodule`
- `bbq.deployed`
- `bbq.static_hidden`
- `bbq.static`
- `campfire_static`
- `campfire`
- `carvable.pumpkin`
- `chineselantern.deployed`
- `cursedcauldron.deployed`
- `electricfurnace.deployed`
- `fireplace.deployed`
- `furnace.large`
- `furnace_static`
- `furnace`
- `hobobarrel.deployed`
- `hobobarrel_static`
- `jackolantern.angry`
- `jackolantern.happy`
- `lantern.deployed`
- `legacy_furnace`
- `refinery_small_deployed`
- `skull_fire_pit`
- `small_refinery_static`
- `tunalight.deployed`
