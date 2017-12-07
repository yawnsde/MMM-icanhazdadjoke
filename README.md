# MMM-icanhazdadjoke

This is a module for the [MagicMirror²](https://github.com/MichMich/MagicMirror/).

Pulls a random joke from icanhazdadjoke.com

## Installation

```
cd ~/MagicMirror/modules
git clone https://github.com/yawnsde/MMM-icanhazdadjoke.git
```

## Using the module

To use this module, add the following configuration block to the modules array in the `config/config.js` file:
```js
var config = {
    modules: [
        {
            module: 'MMM-icanhazdadjoke',
			position: 'bottom_right',
            config: {
                // See below for configurable options
            }
        }
    ]
}
```

## Configuration options

| Option           | Description
|----------------- |-----------
| `maxWidth`        | *Optional* Limit the maximum width. Use any valid int number, for example maxWidth: 300<br>Default is null, so full width required
| `updateInterval`        | *Optional* Update interval, how often a new joke should be fetched <br><br>**Type:** `int`(milliseconds) <br>Default 600000 milliseconds (10 minutes)
