# News

---

### <p style="text-align:left;">Version 0.5 released! <span style="float:right;">18.03.2018</span></p>

---

The most important new feature in this release is support for laminated bows, i.e. bows that consist of multiple layers.
This has been on the list for quite a while and allows for a much wider range of possible bow designs.
As usual there are also various bug fixes, usability improvements and little design changes.

For Windows there is now a 64 bit version available in addition to the 32 bit one.
Download numbers will decide the fate of the 32 bit version in future releases.

For Linux the distribution agnostic download is now an [AppImage](https://appimage.org/) instead of a [snap package](https://snapcraft.io/).

---

### <p style="text-align:left;">Version 0.4 released! <span style="float:right;">04.11.2017</span></p>

---

The main new features for this release are

* Contact handling, which allows the simulation of recurve bows
* Two new simulation results: String force and grip force
* A compatibility layer for opening older bow files. From now on you can expect your files to keep working with new releases, despite the file format changing every now and then.

There are also various smaller and larger bug fixes and other improvements.
Most notably the robustness of the static simulation methods has increased a lot.
Many bow designs that previously would have crashed the simulation are now possible.

---

### <p style="text-align:left;">Version 0.3 released! <span style="float:right;">04.09.2017</span></p>

---

This release introduces a new command line interface for running simulations in batch mode, without opening the GUI.
This way Bow Simulator can be called from other programs for performing more advanced computations like parameter studies and optimizations.

The [user manual](resources.md) has been updated with detailed specifications of the input and output formats and an example for using Bow Simulator with the Python programming language.

---

### <p style="text-align:left;">Version 0.2 released! <span style="float:right;">06.08.2017</span></p>

---

Did I say the previous version was a complete redesign? Well, here's another one.
This time the changes are

* A new tree based bow editor
* A 3d view of the limb geometry
* Many minor improvements and bugfixes

Unfortunately there is also some bad news: No more Mac OS support for now.
I previously used a virtual machine to compile the Mac version of this program, but it stopped working and I couldn't manage to set it up again (Mac OS can be really tricky without Apple hardware).
So in order to not delay this release any further I decided to give up on that for now.

---

### <p style="text-align:left;">Version 0.1 released! <span style="float:right;">25.12.2016</span></p>

---

This is the initial release of Bow Simulator, a complete rewrite and redesign of its predecessor [Bow Simulation Tool](https://sourceforge.net/projects/bowsimulationtool).
It comes with many improvements such as

* A more user-friendly interface
* Improved simulation performance
* Cross-platform support (Windows, Linux, Mac OS X)

The internal redesign of the program lays the groundwork for new features like simulating laminated bows, which is planned for one of the upcoming versions.
Thank you for your interest and stay tuned!
