# oldpersian_xkb_layout

An xkb QWERTY phonetic layout to input Old Persian cuneiform.
You just didn't know you needed it.

# Installation
Copy `oldpersian` to `/usr/share/X11/xkb/symbols/`, then edit
`/usr/share/X11/xkb/rules/evdev.xml`, add this after any of the
layouts.

```
<layout>      
  <configItem>    
    <name>oldpersian</name> 
    <shortDescription>𐎱</shortDescription>            
    <description>Old Persian</description>            
    <languageList>                                           
      <iso639Id>peo</iso639Id>                               
    </languageList>               
  </configItem>                   
</layout>
```

Then restart X by logging out and back in and add the layout 
the way you usually do (GNOME settings or anything else).

# Features

* Plain Old Persian cuneiform straight from the Unicode block.
* Numbers kind of suck, number 5 is missing as a single character.
  It seems that the recommended way to write Old Persian numbers
  is to juxtapose them, e.g. 21 for 3, 2221 for 7, 20-20-10 for
  fifty (without the dashes), and so on. You can of course do
  that.
* For some reason, QT5 apps aren't supported. This is probably
  a QT bug, since QT6 works – although it doesn't render correctly,
  but that's probably a problem on my machine.
