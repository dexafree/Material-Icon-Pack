# Material Icon Pack
This repository contains a full set of png icons, which are directly extracted from Polymer's `Material-Design.ttf` font file.
This icons are provided in the standard Android resolutions: from mdpi to xxhdpi.

The repo also contains the original `Material-Design.ttf` font (with its license), and a ruby script for anyone who needs to export the icons in other sizes.

The script can be run just by running
```
ruby extract.rb <size HxW> <output-folder>
```

In example, in order to get the xxhdpi ones, you would only need to type:
```
ruby extract.rb 96x96 xxhdpi
```

And then you would have all the icons contained in the font, exported to a new folder called `xxhdpi`

The ruby script was based in a previous script I found, made by yukinoraru.

Enjoy the icons!

## Size guide
* mdpi: 32x32
* hdpi: 48x48
* xhdpi: 64x64
* xxhdpi: 96x96

## License
The script is licensed under Apache v2, so basically you can do whatever you want with it. For more info: [See SCRIPT-LICENSE file](https://github.com/dexafree/Material-Icon-Pack/SCRIPT-LICENSE.txt)
