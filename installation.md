- If you run a 64 bit system, in a terminal window do this
**sudo dnf install zlib-devel.i686 ncurses-devel.i686 ant**

- Install libs for mksdcard SDK Tool
**sudo dnf install compat-libstdc++-296.i686 compat-libstdc++-33.i686 compat-libstdc++-33.x86_64 glibc.i686 glibc-devel.i686 libstdc++.i686 libX11-devel.i686 libXrender.i686 libXrandr.i686**

- Install Java development tools
**sudo dnf install java-1.8.0-openjdk-devel.x86_64**
   
- Download the Android Studio package from **http://developer.android.com/sdk/index.html**

- Extract the package (it's ok also the Downloads folder) and relocate the Android Studio folder
**mv /home/yourUserName/Downloads/android-studio /opt**

- Make symbolic lynk for a quick launch
   - Using command line
      - ln -s /opt/android-studio/bin/studio.sh /usr/local/bin/asb
      - exit
   - Using Android Studio (see quick-launch_via_Android_Studio.png)
      - Run Andorid Studio with ./opt/android-studio/bin/studio.sh
      - Menu > Tools > Create Command-line Launcher...
         - Name: asb
         - Path: /usr/local/bin
      - Click OK
   - Using Alacarte (sudo dnf install alacarte)
      - New item under Programming
      - Browse to /opt/android-studio/bin/studio.sh
      - Browse icon to /opt/android-studio/bin/studio.png
   
- Check Java environment
   - echo $JAVA_HOME
   If it isn't /usr/lib/jvm/default-java, type:
   - export JAVA_HOME=/usr/lib/jvm/default-java
   
- Run Android Studio and enjoy it
   - Typing asb in terminal
   - Using Android Studio icon in launcher
