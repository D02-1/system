# Neuen Rechner fürs Entwickeln fit machen
## Windows: 
Damit ihr wie gewohnt mit dem Windowsrechner entwickeln könnt, braucht ihr Windows Subsystem Linux:

1. Installiere *WSL*: 
 
  - Anleitung auf Englisch mit Bildern: https://code.visualstudio.com/docs/remote/wsl-tutorial#_run-in-wsl
   Bis Achschnitt "Python" lesen!

- Anleitung auf Deutsch:  
  1. Einstellungen öffnen
	2. wähle in der Menu *Update und Sicherheit* 
	3. Klicke auf: *Für Entwickler*: **schalte Entwickler modus an**
	4. Systemsteuerung öffnen
		1. Wähle in der Menue *Programme*:
			1. Unterpunkt *Programme und Features*, 
      Unterpunkt:  *Windows features an oder ausschalten*
			2. scrolle zu *Windows subsystem for linux* und wähle Windows subsystem for linux  aus
	   3. **Rechner neustarten**

	5. *Ubuntu*: gehe zu Microsoft Store und suche nach `ubuntu`
		1. installiere die neuste Version (20.04) (Stand 26.05.21)
		2. klick auch *Launch/Starten* => öffnet neuer CLI mit Ubuntu in der Ecke
    
    3. Auf der Ubuntu Kommandozeile 
		1. lege Username (nur kleinbuchstaben sind erlaubt) und Passwort fest (passwort sieht man nicht beim tippen). Merke dir das Passwort, das wirst du immer wieder brauchen. 
	7. Führe folgende Kommandos auf der Ubuntu-Kommandozeile aus, um Pakete zu installieren und  updaten :
		1. `sudo apt update`
		2. `sudo apt upgrade`
		3. Bei Upgrade wirst du gefragt: *"do you want to continue"*: Gib dann ein: `yes`


2. Installiere *Node* (von website  https://nodejs.org/en/)  **ODER** über die Kommandozeiel:  
  apt gibt uns version 10 also führe lieber folgende Kommands aus:

    1. `touch ~/.bashrc` 
    2. `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash` 
    3. **Die Kommandozeile schließen und ein neues Fenster aufmachen!**
    4. `nvm install --lts` um die neuste Version von Node zu instellieren. 
    5. Führe `node --version` aus und du solltest 14.16.1 oder 16.00.0 sehen. 


1. Installiere git und konfiguriere git 
	- ist es schon installiert? git --version, wenn nicht => installieren   sudo apt install git
	- $ git config --list --show-origin
	- $ git config --global user.name "John Doe"
	- $ git config --global user.email johndoe@example.com
	-  $ git config --global core.editor nano
	- git config --list


### Optionales

- Installiere sass `npm install -g sass`
(alt mit sudo)
	- Installiere live-server `npm install -g live-server`
(alt mit sudo)

- Installiere VSC und ändere Einstellungen
	- Remote server: https://code.visualstudio.com/remote-tutorials/wsl/getting-started 
	- Anpassen bei Welcome: Farben, Keybindings (Tastenkürzel)
	- Settings (auf Rad unten links): Auto Save onFocusChange
	- Tab size 2
	- https://code.visualstudio.com/docs/getstarted/tips-and-tricks
- Installiere chrome und firefox
- Installiere Slack
-  Installiere Zoom
- Installiere Postman
- Installiere MongoDB [Link](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-windows/)

  - Lade  der Installer runter.
Auf der Windows- Kommandozeile (nicht bash):
gehe zu `C:\Program Files\MongoDB\Server\4.4\bin`
 und starte den MongoDB server mit `mongo`.
  - lade Mongo Compass runter [hier](https://www.mongodb.com/try/download/compass?tck=docs_compass) und verbinde mit localhost:27017 (Das ist der Default Port von MondoDB). Dann solltest du eine Demo-Datenbank in Compass sehen können.




    

## Mac: 
1. installiere *xcode* vom App-Store. 
2. installiere *homebrew* [link](https://brew.sh/). Das ist ein Package manager für Mac und Linux. Damit lassen sich die meisten  Pakete, die du für  Entwicklung brauchst, installieren. 
3. installiere *node* durch homebrew [node](https://formulae.brew.sh/formula/node#default)
4. *Git*:

	1. Schaue zuerst nach, ob es schon installiert ist! (ist es bei einem Mac meistens). Führe auf die Kommandozeile folgendes aus: `git --version`, wenn es nichts zurückgibt, dann muss  *git* installiert werden:[git](https://formulae.brew.sh/formula/git#default): `brew install git`

    2. Konfiguriere git. Führe auf die Kommandozeile folgendes aus:
	- `git config --list --show-origin`
	- `git config --global user.name "Dein Nutzername"` (Dein Nutzername von GitHub muss in Anführungszeichen stehen)
	- `git config --global user.email johndoe@example.com` (hier ersetzt du die Beispieladresse mit deiner Email-Adresse)
	- `git config --global core.editor nano`
	- `git config --list`

### Optionales
  1. Postman
  2. Installiere MongoDB durch Homebrew:

      - Schreib auf der Kommandozeile: 
      `brew tap mongodb/brew`

      - Überprüfe, dass dein System aktuell ist: 
      `brew tap | grep mongodb`

      - MongoDB sollte aufgelistet sein in der Liste von taps

      - Installieren: 
      `brew install mongodb-community@4.4`

      [Längere Anleitung](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/)

      - Installiere MongoDB Compass: [link](https://www.mongodb.com/try/download/compass?tck=docs_compass) **ODER** Installiere den Extention MongoDB for VS Code (nicht ganz so hübsch)

      
  3. Installiere `sass` global `npm install -g sass`
  4. Installiere live-server `npm install -g live-server` 

  5. installiere Visual Studio Code: 
https://code.visualstudio.com/docs/getstarted/tips-and-tricks

      Ich ändere immer folgende Settings:

      - Costumize bei Welcome: Farben, keybindings (Tastenkürzel)
      - Settings (auf Rad unten links): 
          
        - Auto Save zu `onFocusChange`
        - Tab size 2
	
1. Chrome und Firefox
1. Trello
1. Slack
1. Zoom
1. Importiere alte Lesezeichen von Chrome
1. ev. Dateien vom alten Recher rüberkopieren

    