# screenshot
minimal screenshot script for X

dependencies:
- `shotgun`
- `hacksaw`
- any editor [optional], by default only works with `basicrop`

`shotgun` and `hacksaw` can be replaced with `maim` and `slop`. 
## usage
```sh
# default behavior will take a full screenshot, copy to clipboard, and save to $foto.

# adding "crop" will let you crop or select a window
# "file" will remove clipboard saving
# "clip" will remove file saving
# "clip" followed by "file" just happens to equate to stdout, if you need that
# "-o out.png" will save the image to "out.png"
# "edit" will disregard all other args except "clip", and edit the most recent file in $out
#
# ex: "screenshot crop -o '/tmp/ball.png' file" will capture a crop and send it to '/tmp/ball.png' without saving to your clipboard.

# change $fotoDir and $foto to change your default directory and filename
```
the argument handling is kinda funny but it works.
##
Change this script to suit your needs, if needed. I chose shotgun and hacksaw as the primary tools because they're fast and minimal.
