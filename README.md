# install-Vscode-in-termux
How to install vs code in termux


first install termux from play-store
https://play.google.com/store/apps/details?id=com.termux&hl=en_IN&gl=US

or from fdroid
https://f-droid.org/en/packages/com.termux/   (latest version available here cause play store version has stopped receiving updates)

Note: if you install termux from fdroid link it will download the fdroid apk. So first install fdroid apk then search for termux (Terminal emulator with packages) this one and install it.

After that open termux and type:

termux-change-repo

A prompt will apear just allow it. (if no prompt appears then go to settings and check if the storage permission has enabled or not if not just enable it)

After that open termux and type :

pkg install wget openssl-tool proot -y && hash -r && wget https://raw.githubusercontent.com/EXALAB/AnLinux-Resources/master/Scripts/Installer/Ubuntu/ubuntu.sh && bash ubuntu.sh

It will start dwonload the required files so wait for this to finish

After that type :

./start-ubuntu.sh

Now the ubuntu is running so we have to download vscode 

Check if the wget is installed or not by typing
apt-get install wget

Now type the following command to Download VS Code :

wget https://github.com/cdr/code-server/releases/download/v3.10.2/code-server-3.10.2-linux-arm64.tar.gz

Now extract the file by typing :

tar -xf ./code-server-3.10.2-linux-arm64.tar.gz

Now go to the directory of vscode by typing:

cd code-server-3.10.2-linux-arm64/bin

Now you have to setup a password to use vscode:

export PASSWORD="password"

Now type the following command to run vscode :

./code-server

Now you can run your VSCode by going into your browser and typing :

localhost:8080


here you go now you can run your vscode here.


Thank you.

