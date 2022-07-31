disable_toc: true

<div>
    <p style="float: left;"><img src="img/logo.svg" style="height: 80px; margin: 5px 20px 0px 0px"></p>
    <h1><b>VirtualBow</b></h1>
    <h4>Software for designing and simulating bows</h4>
</div>

---

VirtualBow is a free, open-source software tool for designing and simulating bows.
It gives users an easy way to test and optimize their bow designs before actually building them.
The software provides almost instant feedback about a bow's predicted performance by calculating things like the force/draw curve, limb deformation, stress distributions, arrow velocity and degree of efficiency.

For more details see the screenshots and feature list below or have a look at the [user manual](../files/user_manual.pdf).

---

<a href="img/screenshot_01.png" class="imagelink"><img src="img/screenshot_01_thumb.png" style="height: 125px"></a>
<a href="img/screenshot_02.png" class="imagelink"><img src="img/screenshot_02_thumb.png" style="height: 125px"></a>
<a href="img/screenshot_03.png" class="imagelink"><img src="img/screenshot_03_thumb.png" style="height: 125px"></a>
<a href="img/screenshot_04.png" class="imagelink"><img src="img/screenshot_04_thumb.png" style="height: 125px"></a>

---

## Features

---

**Model Editor**

* Create, load and save bow models
* Edit width, layers, materials and many other properties of your bow

**Solver & Result Viewer**

- Simulates the statics and dynamics of the bow based on the [finite element method (FEM)](https://en.wikipedia.org/wiki/Finite_element_method)
- Static results: Behaviour of the bow when being drawn from brace height to full draw
    - Limb shapes
    - Draw curve
    - Stored energy
    - Stress distribution
    - ...

- Dynamic results: Behaviour of the bow and arrow in motion when the string is released
    - Position, velocity and acceleration of string and arrow
    - Kinetic and potential energy
    - Degree of efficiency
    - ...

**Command Line Interface**

- Run simulations from the command line for advanced use cases
- Call VirtualBow from external programs/scripts to perform parameter studies and design optimizations

**Fully Documented**

- [User Manual](../files/user_manual.pdf): Explains all features of the program and helps you getting started
- [Theory Manual](../files/theory_manual.pdf): Detailed documentation of the internal simulation methods

**Free and Open-Source**

- Released under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl.html)
- Free to use, modify and redistribute
- Anyone can [get involved](contributing.md) in the development

**Cross-Platform**

- [Downloads](download.md) are available for Windows, Linux and macOS