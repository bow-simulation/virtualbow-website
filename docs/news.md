### <p style="text-align:left;">Version 0.7 released! <span style="float:right;">28.05.2020</span></p>

---

The most notable change in this new version of VirtualBow is that the application has been split into the following three independent components:

* *VirtualBow* - Model editor, creates, loads and saves model files
* *VirtualBow Post* - Result viewer, opens and visualizes result files
* *VirtualBow Solver* - Reads a model file and produces a result file

The basic workflow of the program is still very similar, but it is now also possible to save and view simulation results independently from the main application.
Other than that there are many smaller improvements to the user interfaces of both model editor and result viewer.
On the simulation side, several new output results were added, as well as the possibility to take the damping properties of limbs and string into account.

Since Windows 7 reached its end of life in January this year, it is no longer a supported platform for VirtualBow.
Along with that, the 32 bit Windows version was also dropped from the releases.
Another release that unfortunately had to be dropped is the AppImage for Linux.
The approach "one application - one file" just doesn't work very well anymore with the new components.
Hopefully most users can switch to the `deb` or `rpm` packages.
Sorry for any inconvenience this may cause!

As always, a detailed list of changes can be found in the [changelog](https://github.com/bow-simulation/virtualbow/blob/develop/Changelog.md).

### <p style="text-align:left;">Version 0.6.1 released! <span style="float:right;">02.11.2019</span></p>

---

This is just a minor bugfix release and only relevant if you (plan to) use the command line interface on Windows.
It fixes an issue when trying to read the binary output files with Python.

Meanwhile, work on the next major version 0.7 continues as usual.

### <p style="text-align:left;">Version 0.6 released! <span style="float:right;">11.08.2019</span></p>

---

The first thing you might notice is that this project has been renamed to *VirtualBow*.
The old name *Bow Simulator*, even though very descriptive, was a bit uninspired and more of a placeholder anyway.

This latest version now finally supports MacOS, making the software available on all major desktop systems.
Releases for `rpm`-based Linux distributions were also added. Other than that, only minor new features have been introduced, like better width/height interpolation and a more user-friendly way of defining bows with a stiff middle section.
For a complete list of changes have a look at the new [changelog](https://github.com/bow-simulation/virtualbow/blob/develop/Changelog.md).

Most of the work on this version however doesn't affect users directly.
The project has been moved to [GitHub](https://github.com/bow-simulation/virtualbow/) and now uses [Azure Pipelines](https://azure.microsoft.com/en-us/services/devops/pipelines/) to automatically build release files for all supported platforms.
This makes creating and testing new releases much less time-consuming and will hopefully lead to more frequent and regular releases in the future.

### <p style="text-align:left;">Version 0.5 released! <span style="float:right;">18.03.2018</span></p>

---

The most important new feature in this release is support for laminated bows, i.e. bows that consist of multiple layers.
This has been on the list for quite a while and allows for a much wider range of possible bow designs.
As usual there are also various bug fixes, usability improvements and little design changes.

For Windows there is now a 64 bit version available in addition to the 32 bit one.
Download numbers will decide the fate of the 32 bit version in future releases.

For Linux the distribution agnostic download is now an [AppImage](https://appimage.org/) instead of a [snap package](https://snapcraft.io/).

### <p style="text-align:left;">Version 0.4 released! <span style="float:right;">04.11.2017</span></p>

---

The main new features for this release are

* Contact handling, which allows the simulation of recurve bows
* Two new simulation results: String force and grip force
* A compatibility layer for opening older bow files. From now on you can expect your files to keep working with new releases, despite the file format changing every now and then.

There are also various smaller and larger bug fixes and other improvements.
Most notably the robustness of the static simulation methods has increased a lot.
Many bow designs that previously would have crashed the simulation are now possible.

### <p style="text-align:left;">Version 0.3 released! <span style="float:right;">04.09.2017</span></p>

---

This release introduces a new command line interface for running simulations in batch mode, without opening the GUI.
This way Bow Simulator can be called from other programs for performing more advanced computations like parameter studies and optimizations.

The [user manual](resources.md) has been updated with detailed specifications of the input and output formats and an example for using Bow Simulator with the Python programming language.

### <p style="text-align:left;">Version 0.2 released! <span style="float:right;">06.08.2017</span></p>

---

This is another fairly extensive redesign of the user interface.
This time the changes are

* A new tree based bow editor
* A 3d view of the limb geometry
* Many minor improvements and bugfixes

Unfortunately there is also some bad news: No more Mac OS support for now.
I previously used a virtual machine to compile the Mac version of this program, but it stopped working and I couldn't manage to set it up again (Mac OS can be really tricky without Apple hardware).
So in order to not delay this release any further I decided to give up on that for now.


### <p style="text-align:left;">Version 0.1 released! <span style="float:right;">25.12.2016</span></p>

---

This is the initial release of Bow Simulator, a complete rewrite and redesign of its predecessor [Bow Simulation Tool](https://sourceforge.net/projects/bowsimulationtool).
It comes with many improvements such as

* A more user-friendly interface
* Improved simulation performance
* Cross-platform support (Windows, Linux, Mac OS X)

The internal redesign of the program lays the groundwork for new features like simulating laminated bows, which is planned for one of the upcoming versions.
Thank you for your interest and stay tuned!
