# Netbeans Custom Themes
Just a set of themes I decided to port and/or customize for the Netbeans IDE

## Installation
1.  Get the theme (zip archive) you want to install. You can do that in one of
    the following ways.
    * Download it from the [download page](https://github.com/paololus/NetBeans-Custom-Themes/downloads).
    * Create the archive by yourself.
      In this case make sure you zip the _'config'_ folder within the main
      theme folder itself (e.g. _NetBeans-Custom-Themes/Zenburned/**config**_)

2.  Open NetBeans and import the new theme by:
    `Tools => Options => Font & Colors => Import => Browse...` choose the zip archive
    (e.g. Zenburned.zip) `OK`. Now select the `All` option (to import all the settings)
    and finally `OK` again. NetBeans will prompt a window asking you to restart
    the editor in order for the imported settings to be effective. Just confirm.

3.  Enjoy (if everything is ok) or complain (if something wrong happened) =)

## Yesterday Evening
This theme is the result of my tentative to port the theme "Tomorrow Night Eighties"
(https://github.com/ChrisKempson/Tomorrow-Theme) to NetBeans. I soon realized,
though that it would eventually evolve independently form the original theme and
it maybe already did. :)

The theme is mainly oriented to support the syntax for PHP, (X)HTML, JavaScript
and CSS.

I consider this theme still on a very preliminary stage because there is still
much room form improvement.

### Preview
__PHP__

![PHP sample](https://github.com/paololus/NetBeans-Custom-Themes/raw/master/samples/Yesterday-Evening/yesterday-evening-php.png)


## Zenburned
This is just a port of the famous and great Zenburn theme (http://slinky.imukuppi.org/zenburnpage/).

For the colors palette I referred to this very useful page: http://wiki.steam-punk.net/zenburn.

I dedicated about one hour or so to create this theme from scratch (actually from
the default theme which comes with NetBeans 7.1), and I mainly targeted the PHP
syntax. This means that you will definitely find lots of inconsistencies! =)

Obviously any comment and input is welcome!

### Preview
__PHP__

![PHP sample](https://github.com/paololus/NetBeans-Custom-Themes/raw/master/samples/Zenburned/zenburned-php.png)

__Diff__

![PHP sample](https://github.com/paololus/NetBeans-Custom-Themes/raw/master/samples/Zenburned/zenburned-diff.png)

## Diff colors

Unfortunately as of now NetBeans does not store the configuration of the colors for the diff in the same way and place
it does for the others.
As far as I know this configuration is stored in the file `diff.properties` which can be found at the following sample location
`~/.netbeans/7.1/config/Preferences/org/netbeans/modules/diff.properties` (_7.1_ being the version of NetBeans in my case on a GNU/Linux system).
Also note that the colors for the diff are global, meaning that they will be applied indipendently from the active theme you have.

### How-to apply the diff colors

The following procedure worked for me. I hope it will work for you too (let me know if it does not).

1.  __Back up the original file__:
    
    `cd ~/.netbeans/<YOUR NB VERSION>/config/Preferences/org/netbeans/modules/`
    `mv diff.properties diff.properties.bak`

2.  __Replace the original file with the one provided with the theme (only for Zenburned for now)__:
    
    `cp /path/to/new/diff.properties ~/.netbeans/<YOUR NB VERSION>/config/Preferences/org/netbeans/modules/diff.properties`

3.  __Try it!__: the next diff you'll do should use the new colors. In any case restarting the IDE won't hurt.

## Disclaimer
Each one of these themes is provided "AS IS".
Use them at your own risk, do whatever you want and be happy =)
