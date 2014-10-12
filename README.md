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

And then you would have all the icons contained in the font, exported to a new folder called `xxhdpi`.

The ruby script was based in a previous script I found, made by yukinoraru.

Enjoy the icons!

## Size guide
* mdpi: 32x32
* hdpi: 48x48
* xhdpi: 64x64
* xxhdpi: 96x96

## Requirements
The ruby script requires ImageMagick to be installed, in order to recognize the `convert` command.

If you are an OS X user, and have [Homebrew](http://brew.sh) installed, you can install it just by
```
sudo brew install imagemagick
```

## How I did it
I needed some Material icons, and after taking a look around the internet, I couldn't find any icon pack that contained all the icons.
The only thing I found was a bootstrap theme ([Bootstrap Material Design](http://fezvrasta.github.io/bootstrap-material-design/)), which contained nearly every icon adapted to Material Design.

As the theme was hosted on GitHub, I took a look at the insights and found that all the icons shown at the website were extracted from the Polymer's Material Design font.

I downloaded the Material-Design.ttf and the Material-Design.svg fonts, in order to have the main font file (.ttf), and inspect which characters contained information (the svg one, you only have to read the tags).

After that, I only needed to create a script that extracted the glyphs and generate the corresponding .png int the desired resolution.
As I thought, someone had previously done that work, so I found yukinoraru's script, which I adapted in order to extract all the icons.

## License
The script is licensed under Apache v2, so basically you can do whatever you want with it. For more info: [See SCRIPT-LICENSE file](https://github.com/dexafree/Material-Icon-Pack/SCRIPT-LICENSE.txt)
