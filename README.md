Sconvolt Chess, Version 0.99.8, by Orest Sota (Last modified: 1/03/2015 )

A simple cross-platform chess engine + GUI I built in C++ as a hobby. It includes editor mode and switching between difficulty levels.

HOW TO RUN THE PROGRAM - (If you don't want to compile it by yourself but you just want to play)

  - On WINDOWS, Just click on executable named Sconvolt.exe. In some windows 
versions you may be required to run as administrator, in that case right-click on the file "Sconvolt.exe" and click "run as administrator.

  - On LINUX, you need to run "startSconvoltLinux", so change the permissions of the files "Sconvolt" and "startSconvoltLinux" (from terminal, type "chmod u+x Sconvolt", "chmod u+x startSconvoltLinux") then start the program by typing ./startSconvoltLinux (it's a script that executes the file "Sconvolt" by automatically linking the required libraries).


How to play: Click and keep the mouse pressed to move pieces in the board. Click on "Editor" to switch to editor mode where you can define your own board state before playing.
 

HOW TO COMPILE THE PROGRAM FROM SOURCE CODE

The same main file (Sconvolt.cpp) can be compiled for Linux and Windows, (On a Mac too).
To compile this program from source code, you will need to install Allegro 5 libraries.


***** Compile from Linux
  // First compile Allegro 5 from source code
  -> git clone https://github.com/liballeg/allegro5
  -> cd allegro5
  -> mkdir build
  -> cd build
  -> cmake ..
  -> make
  -> sudo make install
  -> sudo ldconfig

  The file to be compiled is Sconvolt.cpp:

  One-liner:
  g++ Sconvolt.cpp -o Sconvolt $(pkg-config --libs allegro-5 allegro_image-5 allegro_dialog-5 allegro_font-5 allegro_ttf-5)



***** Compile from Windows

  - One way is to use the code:Blocks IDE and link it with the Allegro programming libraries.
  for further information on how to set up the compiler for windows, this link can be followed:
  http://wiki.allegro.cc/index.php?title=Code::Blocks


