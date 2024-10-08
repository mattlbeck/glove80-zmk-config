# Glove80 personal config

This is my personal configuration for the glove80 keyboard. It is a work in progress!

For much of the changes I am using nickcoutsos' fantastic web app https://nickcoutsos.github.io/keymap-editor/

## Resources
- The [official MoErgo Glove80 Support](https://moergo.com/glove80-support) web site. Glove80 documentation and other technical resources.
- The [official MoErgo Discord Server](https://moergo.com/discord). Instant conversations with other Glove80 users.

- The [official ZMK Documentation](https://zmk.dev/docs) web site. Find the answers to many of your questions about ZMK Firmware.
- The [official ZMK Discord Server](https://discord.gg/8cfMkQksSB). Instant conversations with other ZMK developers and users. Great technical resource!

- The [official Glove80 ZMK Distribution](https://github.com/moergo-sc/zmk). Repositiory for ZMK firmware customized for Glove80. 
 
## Instructions
1. Log into, or sign up for, your personal GitHub account.
2. Create your own repository using this repository as a template ([instructions](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template)) and check it out on your local computer.
3. Edit the keymap file(s) to suit your needs
4. Commit and push your changes to your personal repo. Upon pushing it, GitHub Actions will start building a new version of your firmware with the updated keymap.

## Firmware Files
To locate your firmware files and reflash your Glove80...
1. log into GitHub and navigate to your personal config repository you just uploaded your keymap changes to.
2. Click "Actions" in the main navigation, and in the left navigation click the "Build" link.
3. Select the desired workflow run in the centre area of the page (based on date and time of the build you wish to use). You can also start a new build from this page by clicking the "Run workflow" button.
4. After clicking the desired workflow run, you should be presented with a section at the bottom of the page called "Artifacts". This section contains the results of your build, in a file called "glove80.uf2"
5. Download the glove80.uf2
6. Flash the firmware to Glove80 according to the user documentation on the official Glove80 Glove80 Support website (linked above)

Your keyboard is now ready to use.

## Keymap Guide

The keymap is purely for MacOS and is a work-in-progress that is heavily integrated with my hammerspoon configuration and additional tools that I used.

 - See my dotfiles repo: 

What follows are notes on each layer and whether it  it currently in use

 1. colemak-dh. Keyboard layout with some frequently used symbols along the bottom
 2. sympad. A combination of symbols and a numpad on the right hand side
 3. cursor: Cursor navigation with copy/paste functions on the inner columns
 3. mouse: mouse control, clicking, and scrolling with copy/paste on the inner columns
 4. screen_nav: uses [Rectangle](https://rectangleapp.com/) to position and tile windows with a focus on widescreen monitor usage. Then there are keys to navigate tiled windows and tabs within tabbed programs.
 5. switcher: unused
 6. window: unused
 7. Amethyst: unused
 8. magic: glove80 magic functions - bluetooth, RGB, bootloader access and reset.

 Additional notable features:
  - I have modifiers lining the homerow when using layer 0, cursor, and mouse layers.

## Keymap SVG

This repo also contains a build pipeline to create SVGs of the keyboard layout and all its layers. This uses the python utility keymap-drawer to generate the SVGs from the keymap.json file. The resulting SVG is commited as keymap.svg in the root of this repo.