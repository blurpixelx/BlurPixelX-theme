This Repo assumes you've created icons or themes for opencore. Resources to referenced documentation is listed below. Message me on reddit for help!

BlurPixelX
 
<img width="3440" height="1440" alt="blurpixelx-theme" src="https://github.com/user-attachments/assets/04f29755-edd8-4ebc-b5c7-8888b2774f65" />
Please make your own copy - Do not request access to edit this one. Figma allows you to have your own local file.

Opencore Theme inspired for Tahoe using Liquid Glass

Figma link: https://www.figma.com/design/yQmG4Y1hzpiVzfgyA3yppJ/Hackintosh-Theme--BlurPixelX?node-id=1-1632&t=4OeKic8etLmCTdYC-1

Credit to velickovicdj for creating original icons and theme.

Forked by BlurPixelX for customizing background image on figma and modifying icons using Liquid Glass.

Not all icons have been curated. Only essentials.

This script will convert all images to icons in your icnspack folder (Background-1.png + Background.png into Background.icns)

```bash
#!/bin/bash
icons=("Background" "HardDrive" "BtnFocus" "Selected" "SetDefault" "Windows" "Selector" "Tool" "Shell" "AppleRecv")
for name in "${icons[@]}"; do
  echo "Packing $name.icns from $name-1.png and $name.png"
  ./icnspack "$name.icns" "$name-1.png" "$name.png"
done
echo "✅ All icons have been packed."
```

Resolution for specific monitor sizes is not defined. 
You will have to export it to your proper resolution from your monitor. 
Figma is pretty complex. I’ve modified the background to scale and adapt. 
Shouldn’t be too hard to get the right size for you.

Modify the text fields with your hardware specs.

Leave the declaration of gratitude, but feel free to remove it if you don’t see fit.
Under Background, Art board 1 is the main component. 

Art board 2 is a mirror of art board 1. Do not modify Art board 2.

You’ll need 1 and 2 (2x in size) in order to create a proper Background.icns

Learn how to create icons for OC

https://dortania.github.io/OpenCore-Legacy-Patcher/ICNS.html#custom-opencore-icons

Original Theme Download: velickovicdj/EnterTwilight

https://github.com/velickovicdj/OpenCanopy-EnterTwilight
