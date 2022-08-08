# FWB Vita
TwistedScarlett60's Friendship with Benefits eroge Vita port.
Made using [Ren'Py PSVita Distribution Tool](https://github.com/SonicMastr/renpy-vita/releases/tag/v1.0)

![image](https://cdn.cloudflare.steamstatic.com/steam/apps/1299370/capsule_616x353.jpg?t=1606926788)

Game Page: https://store.steampowered.com/app/1299370/Friendship_with_Benefits/

# Known issues
There is an issue with name input

# How to use the distribuiton tool
1. Put the game folder inside the Ren'Py PSVita Distribution Tool folder. Exe: ```...\Ren'Py PSVita Distribution Tool\DDLC```
	- To reduce the size of the VPK and be able to distribute your port without piracy, remove the contents of the "game" folder inside your game.
	<br />Exe: ```...\Ren'Py PSVita Distribution Tool\DDLC\game```
2. Create a "sce_sys" folder inside the folder of the game, and inside that create a "livearea" folder with a "contents" folder inside.
	- It shold look something like this:
	<br />```Ren'Py PSVita Distribution Tool\DDLC\sce_sys\livearea\contents```
3. Creat the assets for the live area following this parameters
	- All images MUST be in 8-bit color depth
	- "sce_sys" Folder
		- icon0.png (128x128) [app icon]
		- pic0.png (960x544) [app opening screen]
	- "contents" Folder
		- bg.png (840x500) [app card background]
		- startup.png (280x158) [app logo]
		- template.xml [card template] you can get the code for a basic one [here](https://github.com/SKGleba/Vita-NDP/blob/master/sce_sys/livearea/contents/template.xml). them save it as "template.xml
4. Open the "Ren'Py PSVita Distribution Tool.exe". if you did everything right, the project should be listed at the left side.
<br />Select your project, if a red warning shows up at the botton, probably a asset is missing. If not Proceed to add the app information.
	- Application Name: ```At your choice```
	- Title ID: ```9 character at your choice``` Exe: ```FWB00000```
		- Make sure it doesn't conflict with any existing game or homebrew
	- App Version: It should follow this extructure ```XX.XX``` Exe:```01.20```
If all the information is filled correctly the "Build VPK" button should become avaliable. Click it to build the VPK and wait for the confirmation text to apear.

5. Your VPK will be on the dist folder, instal it on your vita, and copy the contents of the game folder inside the application folder. The name of the folder is the ID you gave it earlier.
<br />Exe: ```ux0:\app\FWB000001```
	-The instalation may take a while to complete
	-If you get a error on the VPK instalation, probrabily is something wrong with the assets, the title ID or the App Version.
