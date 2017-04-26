# UK International Keyboard

## Some information

Hi!
I'm a spanish person.

Some time ago, I bought a keyboard and a laptop in a web store in UK. Obviously they come with UK keyboard layout.

I do not like use a different keyboard layout than the proper of the device, so I searched through the Internet, and I found a custom Windows design that I love.

![Original keyboard layout](http://www.zolid.com/uk-intl-kb/UK-Intl%20WEur%20kb%20(v2.0).png) 
###### [The image is property of the original developer](http://www.zolid.com/uk-intl-kb/index.htm)


As a programmer I spend almost all my time in linux so I decided to porting the project to xkb.

## How to install

1. Clone the repository where you want
2. Open the repo folder
3. Open a terminal in this folder and run as root
```
# cat uk-intl-kb >> /usr/share/X11/xkb/symbols/gb
```
4. Open as root /usr/share/X11/xkb/rules/evdev.xml with your favourite text editor
5. Search layoutList -> layout -> configItem -> gb
6. Go to its variantList and add

```
 <variant>
     <configItem>
         <name>intlextd</name>
         <description>English (International, Extended)</description>
     </configItem>
 </variant>
```
7. Select "English (International, Extended)" in your keyboard layout
8. Enjoy

## Original project and thanks

So many thanks to James Campbell for the original project, you can download it from here: [UK International Keyboard for Windows](http://www.zolid.com/uk-intl-kb/index.htm)
