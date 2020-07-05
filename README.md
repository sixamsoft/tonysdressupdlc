# Tony's Dress Up DLC

This is a prototype DLC template for my [dress up game](https://github.com/tonytins/tonysdressup).

## How it works

```text
.
+-- /sprites
|	 +-- /clothes
+-- /resources
|   +-- character.tres
+-- scripts
|   +-- world.gd
+-- /scenes
|	 +-- /clothes
|		  +-- /base
|   +-- /dlc
|   	+-- shirts.tscn
```

This project contains the core components of Tony's Dress Up. In it are the base button scenes with their functionality, located in ``res://scenes/clothes/base`` and ``res://scripts/clothing``, needed for changing the character.

Following the base game, you put all clothing sprites in ``res://sprites/clothes``, inherent from one of the button bases, change the button sprite with your sprite, save it, and place that button scene in ``shirts.tscn``. It's recommended to put all clothing scenes in ``res://scenes/clothes``.

The base game will look for ``shirts.tscn``, ``pants.tscn``, ``undies.tscn`` and ``accessoires.tscn``. It'll load these scenes and include all of it's nodes into each respective tab. The base game will **not** use the DLC's version of the core components because their the same.

Finally, you only need to export the PCK. You can do this by going to ``Export > (any template) > Export PCK/Zip``.

​
## Getting Started

### Prerequisites

- Godot Engine 3.2

## Authors

- **Anthony Wilcox** - *Initial work* - [tonytins](https://github.com/tonytins)

## License

The source and assets are licensed under the MIT License and CC-BY, respectfully - see the [LICENSE](LICENSE) and [ASSET-LICENSE](ASSET-LICENSE) for more details.