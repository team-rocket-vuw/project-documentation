**Project Charter**

**Rocket Avionics System**

**----------------------------------------------------------**

**Project Overview:**

Design and implementation of an actively stabilised, open-sourced avionics system. The goal of the rocket is to travel in the most upright trajectory possible whilst transmitting telemetry data (at least one-way communication) for retrieval of the rocket.

**Project Justification:**

By utilising both the project client’s resources, as well as our own, we will gain experience in both the field of avionics as well as project management. By adhering to good project management principles, we will create a good product, and doing so open-source, will allow others to extend upon our work.

**Project Objectives:**

* Launch an actively stabilised rocket

* Open source all components of rocket

* Learn the fundamentals of project management

* Transmit telemetry data

* Land rocket within a reasonable distance of target

**Project Constraints:**

* Fit within a 2.9cm-6cm diameter

* Implement some form of data collection

* All components of the final project, both hardware and software, must be fully open-source. (This includes simulation, component design, documentation, tools and code)

* Adhere to legal requirements (CAA and DOC)

* Find a viable launch site

**Project Considerations:**

* Parameter maximisation and control

* which parameters are we going to maximise/control

* Horizon sensing

* Magnetic field

**Project Risks:**

* Time

* Budget

* Knowledge

* Scope

**Project Timeline:**

Start date: *14/03/2016*

Project initiation document: 13/04/2016

Project achievement presentations: (Exam Period)

Finish date: *15/11/2016*

**Project Milestones:**

* Middle trimester break progress report

* Initial test flight (Potentially smaller version of final rocket)

    * Utilise this for basic sensor positioning and logging (Data dump)

**Stakeholders:**

Client: *Andre Geldenhuis*

Champion: *Holly Ade-Simpson*

**_Project Communication:_**

Communication platform: **Slack**

Meeting with Andre two weeks from now: 10am 30/03/16

**Project Budget:**

<table>
  <tr>
    <td>From:</td>
    <td>University</td>
    <td>Client</td>
  </tr>
  <tr>
    <td>Amount:</td>
    <td>$200.00</td>
    <td>Unspecified</td>
  </tr>
  <tr>
    <td>TOTAL:</td>
    <td>$100.00</td>
    <td></td>
  </tr>
</table>


**Project Management Strategy:**

In place of a project manager, it has been decided that each member of the team will micromanage their own time and workload. Weekly meetings will be held to help make sure everyone is on task, and has every resource they need available to them.

**Project Roles & Responsibilities:**

* Secretary (Minutes & Agendas)

* Telemetry

* Sensor Characterisation

* Rocket control

* Parachute controls

* Software

    * Ground controls

    * Data formatting

    * GUI

    * Networking

    * Git-flow

**MISC**

Set up google calendar

Android phone - hack it for remote recovery

Parachutes?

How are we going to microcontroller? SMALL?? Camera?

Calibration on ground

**Andre halp:**

**What is the client's key motivations? - Is it get as high as possible, or create a viable low cost solution, or have a rocket that is self-landing, etc? How high/how fast?**

The controller - PID - keep the rocket pointing up. Want it to stay pointing up as much as possible. Telemetry to find it. K-motor - start with little motors.

Want control system to be light as can be. Data collection - logging of sensors onto SD card or flash. HAM license? Low BAUD rate higher band-width 

**Are we going to try and finish the rocket, or are we going to get as far as we can in the most organised manner we can, so as to most easily allow others to work on this project in the future?**

Not the end of the world if we don’t finish it.

**What sort of documentation does the client want to be kept and to what specific level?**

Markdown on GitHub, thought processes - keep track of stuff that didn’t work and why you made the decisions you did.

**What do you have already (hardware (launch pad?), simulations, communications with external parties/stakeholders)?**

Not much - three years ago, out-dated equipment - has off-the-shelf avionics boards. Motors I200 K700 and some single-use Gs. Make sure you use a really common motor

**Have you launched rockets before? Who did you talk to/what permissions did you get? Where did you do it?**

All done down in Christchurch - Wairarapa; easy to get CAA (ten-minute window, one week in advance), private company called AirWays, call air-traffic control the morning of/ directly before- fire risk - must manage that. Pyrotechnic ejection charges are dangerous - watch out for automatic firing. Must be at least 4km (more like 8km) away from airport. Can fly using smaller motors in Wellington area. 

**Problems you've encountered with previous launches?**

^^

**Open-source tool chains?**

Key Cad for PCB, chibios, Arduino is fine, openS CAD, GCC for compiling, FreeCAD, python, Julia, python (numpy) - can prototype in Matlab but must have final product in python

**How do you feel about us finding our own external funding? - If need be. (Say V or redbull etc.)**

Happy for that, has some money and equipment

**People who have tried this/are trying this:**

NZ Rocketry Association OpenRocket

Worry with 3D printing: get soft because heat of motor

Smaller motor in bigger shell = less heat to fins so doesn’t matter

Barometer = good way of deploying parachute BUT have to worry about speed-of-sound issues. Accelerometer = detect when probably past speed of sound and don’t deploy parachute.

Use the raven to test what happens when go past speed of sound and data log

Small motors will not reach past speed of sound for long

Mobius cams, canards = have cameras pointing down at them

Design rocket to be passively stable so if stabilisation stops it’s not that much of an issue

Outreach stuff? Build super simple implementation which can fly at a school?

Teensy is an ARM we could use Mbed

