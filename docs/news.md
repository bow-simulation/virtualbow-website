disable_toc: true

---

### Version 0.10.0 released! <span style="float:right;">29.08.2026</span>

---

This release has been in the works for a long time and is one of the largest updates so far.
While there are also some new features and improvements in the user interface, the main focus of this release has been the internal simulation methods and their verification.
Here is a selection of the most important changes:

* **A redesigned solver**: The simulation has been rewritten from scratch, with numerous improvements to accuracy and performance.
Most of the numerical methods are now covered by verification tests, including comparisons of the static and dynamic bending solutions with the third-party finite element package [GXBeam](https://flow.byu.edu/GXBeam.jl/stable/).
The new solver also provides more detailed error messages for invalid input and failed simulations.

* **New results**: The new solver also provides a number of additional outputs, such as the stiffness of the force/draw curve, the string angles, the energy lost to damping and a detailed energy breakdown for the moment the arrow leaves the bow.

* **Material strength**: Materials can now be given tensile and compressive strengths as well as a safety margin, so the result viewer can indicate when a layer is stressed beyond its permissible limit.

Other minor improvements include the option to define the draw length according to the AMO convention and the arrow mass in grains per pound.
The complete list of changes can be found in the [changelog](files/user-manual/changelog.html).

---

### Version 0.9.1 released! <span style="float:right;">21.11.2022</span>

---

This is a bugfix release that introduces no new features, but fixes the following two issues:

* Wrong unit label in the results for string length
* Problems with the computation of the limb geometry that sometimes lead to unwanted sharp/pointy limb tips

Both of those are also listed in the [changelog](https://github.com/bow-simulation/virtualbow/blob/develop/CHANGELOG.md#version-091).

---

### Version 0.9 released! <span style="float:right;">22.08.2022</span>

---

It has been a while since the last release, but this new version introduces several important features that have been on the list for a long time.
Particularly the following three points:

* **Support for units**: The units of all input and output data are now configurable, including both SI and US units. Dimensions, for example, can now be entered in millimeters, centimeters or inches instead of meters and the draw force can be displayed in pounds instead of newtons.

* **A new way to define the bow profile**: The profile curve is no longer only based on length and curvature. Instead there are now various segment types like lines, arcs, spirals and splines that can be combined by users. This is only a first minimal version, though, and will be extended in the upcoming releases.

* **A new layout of the bow editor**: The properties of the bow are no longer shown and edited via different pop-up dialogs. The new layout uses fixed panels instead that show the properties currently selected in the model tree.

Other notable new features besides those are:

* An option to overlay images on plots for easier comparison
* Plot contents can be exported as `CSV` for easier exchange with external spreadsheet programs
* Number input fields accept arithmetic expressions, like `(5*5 + 8)/2`
* Material properties can be edited separately from the layers, and the colors are now user-defined

And of course there are also the usual bug fixes and minor changes, all of which are listed in the [changelog](https://github.com/bow-simulation/virtualbow/blob/develop/CHANGELOG.md#version-090).

---

### Version 0.8 released! <span style="float:right;">13.03.2021</span>

---

This release adds various smaller features and improvements, such as:

* A new arrow clamp force that prevents the arrow from leaving the string too early
* New icons for the toolbar and model tree as well as other visual changes
* Improvements to the presentation of some of the output results
* Several bug fixes and minor improvements

The complete list of changes can be found in the [changelog](https://github.com/bow-simulation/virtualbow/blob/develop/CHANGELOG.md#version-080).

---

### Version 0.7.1 released! <span style="float:right;">28.05.2020</span>

---

This minor release fixes two issues that prevent VirtualBow from being usable on macOS, as well as another issue on Windows where the simulation would fail for certain input parameters.

As always, the exact changes can be found in the [changelog](https://github.com/bow-simulation/virtualbow/blob/develop/CHANGELOG.md#version-071).

---

### Version 0.7 released! <span style="float:right;">12.05.2020</span>

---

The most notable change in this new version of VirtualBow is that the application has been split into the following three independent components:

* *VirtualBow* - Model editor, creates, loads and saves model files
* *VirtualBow Post* - Result viewer, opens and visualizes result files
* *VirtualBow Solver* - Reads a model file and produces a result file

The basic workflow of the program is still very similar, but it is now also possible to save and view simulation results independently from the main application.
Other than that, there are many smaller improvements to the user interfaces of both model editor and result viewer.
On the simulation side, several new output results were added, as well as the possibility to take the damping properties of limbs and string into account.

Since Windows 7 reached its end of life in January this year, it is no longer a supported platform for VirtualBow.
Along with that, the 32-bit Windows version was also dropped from the releases.
Another release that unfortunately had to be dropped is the AppImage for Linux.
The approach "one application - one file" just doesn't work very well anymore with the new components.
Hopefully most users can switch to the `deb` or `rpm` packages.
Sorry for any inconvenience this may cause!

A detailed list of changes can be found in the [changelog](https://github.com/bow-simulation/virtualbow/blob/develop/CHANGELOG.md#version-070).

---

### Version 0.6.1 released! <span style="float:right;">02.11.2019</span>

---

This is just a minor bugfix release and only relevant if you (plan to) use the command line interface on Windows.
It fixes an issue when trying to read the binary output files with Python.

Meanwhile, work on the next major version 0.7 continues as usual.

---

### Version 0.6 released! <span style="float:right;">11.08.2019</span>

---

The first thing you might notice is that this project has been renamed to *VirtualBow*.
The old name *Bow Simulator*, even though very descriptive, was a bit uninspired and more of a placeholder anyway.

This latest version now finally supports macOS, making the software available on all major desktop systems.
Releases for `rpm`-based Linux distributions were also added. Other than that, only minor new features have been introduced, like better width/height interpolation and a more user-friendly way of defining bows with a stiff middle section.
For a complete list of changes, have a look at the new [changelog](https://github.com/bow-simulation/virtualbow/blob/develop/CHANGELOG.md).

Most of the work on this version, however, doesn't affect users directly.
The project has been moved to [GitHub](https://github.com/bow-simulation/virtualbow/) and now uses [Azure Pipelines](https://azure.microsoft.com/en-us/services/devops/pipelines/) to automatically build release files for all supported platforms.
This makes creating and testing new releases much less time-consuming and will hopefully lead to more frequent and regular releases in the future.

---

### Version 0.5 released! <span style="float:right;">18.03.2018</span>

---

The most important new feature in this release is support for laminated bows, i.e., bows that consist of multiple layers.
This has been on the list for quite a while and allows for a much wider range of possible bow designs.
As usual there are also various bug fixes, usability improvements and little design changes.

For Windows there is now a 64-bit version available in addition to the 32-bit one.
Download numbers will decide the fate of the 32-bit version in future releases.

For Linux the distribution-agnostic download is now an [AppImage](https://appimage.org/) instead of a [snap package](https://snapcraft.io/).

---

### Version 0.4 released! <span style="float:right;">04.11.2017</span>

---

The main new features for this release are:

* Contact handling, which allows the simulation of recurve bows
* Two new simulation results: String force and grip force
* A compatibility layer for opening older bow files. From now on you can expect your files to keep working with new releases, despite the file format changing every now and then.

There are also various smaller and larger bug fixes and other improvements.
Most notably the robustness of the static simulation methods has increased a lot.
Many bow designs that previously would have crashed the simulation are now possible.

---

### Version 0.3 released! <span style="float:right;">04.09.2017</span>

---

This release introduces a new command line interface for running simulations in batch mode, without opening the GUI.
This way, Bow Simulator can be called from other programs for performing more advanced computations like parameter studies and optimizations.

The user manual has been updated with detailed specifications of the input and output formats and an example for using Bow Simulator with the Python programming language.

---

### Version 0.2 released! <span style="float:right;">06.08.2017</span>

---

This is another fairly extensive redesign of the user interface.
This time the changes are:

* A new tree-based bow editor
* A 3D view of the limb geometry
* Many minor improvements and bug fixes

Unfortunately, there is also some bad news: No more Mac OS support for now.
I previously used a virtual machine to compile the Mac version of this program, but it stopped working and I couldn't manage to set it up again (Mac OS can be really tricky without Apple hardware).
So in order to not delay this release any further I decided to give up on that for now.

---

### Version 0.1 released! <span style="float:right;">25.12.2016</span>

---

This is the initial release of Bow Simulator, a complete rewrite and redesign of its predecessor [Bow Simulation Tool](https://sourceforge.net/projects/bowsimulationtool).
It comes with many improvements such as:

* A more user-friendly interface
* Improved simulation performance
* Cross-platform support (Windows, Linux, Mac OS X)

The internal redesign of the program lays the groundwork for new features like simulating laminated bows, which is planned for one of the upcoming versions.
Thank you for your interest and stay tuned!

<br>