# debian-nonfree
Quelques commandes pour que votre Debian 11 devienne une Debian 11 NON-FREE !

A few commands to make your Debian 11 a NON-FREE Debian 11!

# Description
Installez tous les micrologiciels non libres de Debian 11.

Avant de continuer, assurez-vous que | MAIN NON-FREE CONTRIB | sont ajoutés aux dépôts de votre système.
Ceux-ci sont généralement disponibles dans les paramètres de votre gestionnaire de paquets.
Ou vous pouvez modifier vos sources directement avec <sudo nano /etc/apt/sources.list>
Ajoutez MAIN NON-FREE CONTRIB à la fin de chaque ligne.

Exemple : deb http://deb.debian.org/debian/ bullseye main non-free contrib

Copier le fichier <firmware.list> dans votre répertoire personnel.

Ouvrez une instance "Terminal" à cet endroit.

Exécutez les commandes suivantes pour activer et installer...

* sudo dpkg --add-architecture i386 
* sudo apt-get update
* sudo apt-get install dselect
* sudo apt-get install $(cat firmware.list | awk '{print $1}')

----------------------------------------------------------------------

Install all non-free Debian 11 firmware.

Before continuing, make sure that | MAIN NON-FREE CONTRIB | are added to your system repositories.
These are usually available in your package manager settings.
Or you can edit your sources directly with <sudo nano /etc/apt/sources.list>
Add MAIN NON-FREE CONTRIB at the end of each line.

Example: deb http://deb.debian.org/debian/bullseye main non-free contrib

Copy the <firmware.list> file to your home directory.

Open a "Terminal" instance there.

Run the following commands to enable and install...

* sudo dpkg --add-architecture i386 
* sudo apt-get update
* sudo apt-get install dselect
* sudo apt-get install $(cat firmware.list | awk '{print $1}')

# Demonstration/Démonstration
- https://youtu.be/CQ9kPMaeFts
