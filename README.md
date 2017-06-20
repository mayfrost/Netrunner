# NetRunner

### We are making a web browser!
<img height="300" src="https://github.com/mayfrost/Netrunner/blob/master/netrunner-moon.png">

In the face of recent changes in Firefox and Chrome some anons were asking for a /g/'s perfect web browser, we collected the most wanted here and plan on continuing with the creation.

To contribute follow the WORK PLAN and get to programming!

## Main repo
https://git.teknik.io/eti/netrunner
## Mirrors
https://github.com/5yph3r/Netrunner
http://magicpackets.net:3000/proudfeet/netrunner (currently down)
## IRC
\#/g/netrunner @ Rizon: https://qchat.rizon.net/?channels=/g/netrunner

## TODO:
- Host project at savannah.nongnu.org
- Set bug tracker, website, and mailing list in Savannah.

## WORK PLAN
1. Browse the links2 source code (you can use Ctags or GNU GLOBAL for tagging functions and files).
2. Open API to future javascript integration (by an independent engine?).
3. Dig the javascript enabled version 2.1pre28 of links2 if you are curious.
4. Expose API and give (scripting) access to just about everything.
5. Create a scripting engine for every accessed interface (vimscript-like?).
6. Create a switch by profiles for incoming and outgoing connections (uBlock-like).
7. Create profiles generator for user-agent and canvas fingerprint, with manual option for the user-agent.
8. Give control over the DOM, use folders for each site to be manually edited (use a hierarchical structure to cover subsites).
9. Include cache/tmp/cookies/logs options like read only cache and local CDN emulation.
10. Implement a link grabber for every link available to be parsed by the scripting interface.
11. Work with the links2 ncurses interface to support simple tree style options for everything (adblocking and tabs in the future).
12. Implement tabs and add tree style tabs in ncurses.
13. Work in the tree style bookmark management with ncurses.
14. Add a javascript engine.
15. Work in the framebuffer graphics rendering.
16. Add the rest of the features.

## FEATURES
- Granular control over incomming traffic like Policeman (more control than uMatrix in this particular subject).
- Granular control over outgoing traffic like Tamper Data or like Privacy Settings (the addon).
- Easy switch to preset profiles for both like uBlock Origin for incomming traffic and Privacy Settings for outgoing traffic.
- Random presets generator for things like "user-agent" and "canvas fingerprint".
- Custom stylesheets like Stylish.
- Userscript support like Greasemonkey.
- Cookie management like Cookie Monster.
- HTTPS with HTTP fallback and ports management like Smart HTTPS and HTTPS by default.
- Proxy management like FoxyProxy.
- "Open with" feature to use an external application, like for using a video player with youtube-dl and MPV, or for text input with a text editor, and for other protocols like ftp and gopher, and even as a file picker.
- Local cache like Decentraleyes and Load from Cache.
- Option to turn off disk usage for all data (cache, tmp data, cookies, logs, etc.), or/and make cache read only.
- All this in a per site basis.
- URL Deobfuscation like "Google search link fix" and "Pure URL".
- URI leak prevention like "No Resource URI Leak" and plugin enumeration prevention by returning "undefined".
- Keyboard driven with dwb features like vi-like shortcuts, keyboard hints, quickmarks, custom commands.
- Optional emacs-like keybindings (maybe default for new users to have an easier time?).
- Non-bloated smooth UI like dwb.
- Configuration options from an integrated command-line (with vimscript-like scripting language?).
- A configuration file like Lynx.
- Send commands to the background to be optionally displayed in an optional interface, as to use wget web crawling feature like a DownThemAll, and to use and watch other batch commands.
- A way to import bookmarks from other browsers like Firefox.
- Search customization like surfraw, dwb funtions or InstantFox Quick Search, and reverse image search like Google Reverse Image Search.
- Written in C.
- Low on dependencies.
- GPL v3+.
- Framebuffer support like NetSurf for working in the virtual terminal (TTY).
- Actual javascript support so we can lurk and post in 4chan.

## FAQ
-**Why teknik.io?**  
We plan on moving to savannah.nongnu.org. There is a github mirror too.  
-**Why links2?**  
Enough features and the API seems more friendly.  
-**Why not netsurf?**  
Good rendering but not for DOM updates, plus dependencies gave problems.  
-**Will it have tree style tabs?**  
Yes, but not up in the priorities.  
-**Will it be crossplatform?**  
Already is.  
-**Will you use a separate javascript engine?**  
We're debating this.  
-**Will you use a separate layout engine?**  
We can consider it once we dig up more the code?  
-**Will you use netsurf layout engine?**  
Might be a problem because of the DOM (not enough information).  
-**Will you use webkit/blink/servo?**  
No.  
-**Will it it have vim keys?**  
Yes.  
-**Will it have "graphics"?**  
Yes. We are planning to run the program in terminal using the frame buffer for graphics, but Links2 also comes with directfb, X server, SVGA and other graphics drivers.  
-**Will it have an adblocker.**  
Yes.  
