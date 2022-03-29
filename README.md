# SonicTimeTwisted-Vita
Unofficial Vita port of a Sonic Fan Game Made in Game Maker Studio 1

Made with G*Maker by SilicaandPina

***Make sure you have PSVShell installed and everything overclocked for this to run at a framerate anywhere near playable!***

**Right now, you will need to do the following for input to work**
1. Install and launch the application so it can generate the configuration files. Let it get to the epilepsy warning screen, and then exit.
2. Open Vitashell
3. Navigate to ux0:/user/00/data/STTV00001 (but don't enter the directory yet)
4. Press Δ, and select "open decrypted"
5. Select "settings.ini"
6. Scroll down to the section called [input]
7. Change the line method="1.000000" to read method="2.000000"
8. Save your changes

I'm going to try to find a workaround for this, don't worry!

**Known Issues**
- Some graphical glitches
- Game will appear to freeze when it's trying to load a lot of data at once (e.g. the Attraction Attack Act 1 intro cutscene)
- Game is laggy, even when overclocked. I have no idea how to fix this right now, so if anyone wants to help me out, I will gladly accept PRs

**Plans for the Future**
- Make the default input method the gamepad
- Mitigate lag (maybe by changing the target framerate from 60FPS to 30FPS? The game won't look as smooth, but it will run fast enough to be enjoyable)
- Make nicer-looking livearea assets

**Building (Windows only)**
- Obtain a copy of G*Maker (Google is your friend)
- Clone this repo, either by using Git or by downloading a .zip
- Point G*Maker to the .gmx file, and the assets within the Livearea folder. It will yell at you for bg0.png not being the right size. Ignore this.
- Make sure GM Version is set to 1.4.9999
- Set "Download More RAM" to +109MiB (otherwise the Attraction Attack cutscene, and presumably any other cutscene, will look like a slideshow)
- Set the TitleID and Title to whatever you want
- Obtain a copy of psp2cgc.exe (again, Google)
- Click "Make VPK

Note:
 - The soundtrack, "Dueling Ages" by Hinchy et al. is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by-nc-sa/4.0/.
 - The Linux and Windows builds include a gamepad mapping database from the SDL_GameControllerDB project: https://github.com/gabomdq/SDL_GameControllerDB. To view a copy of the project's license, visit https://github.com/gabomdq/SDL_GameControllerDB/blob/master/LICENSE.
 - The database has also been preprocessed with a script by @offalynne https://gist.github.com/offalynne/e0a887556e8120390fc86c944e6861bf to make it compatible with Studio 1.4.9999.
