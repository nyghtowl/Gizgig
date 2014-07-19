Gizgig
=====

Project: LeapMotion driving an Arduino on Parallax wheels or Arduino on wheels

This repo expands on work done in Silicon Chef/LeapRobo & Electric Imp Hackathons.



Team Members:

* Kelley Robinson
* Kara Louie
* Chris Meona
* Meggie Mahnken
* Melanie Warrick

Tech:

* Arduino Uno
* Parallax Wheel Shield
* Leap Motion
* Python on Leap
* C on Arduino
* Passed values through serial port with the Leap and Arduino connected through USB
* CLI Activation:python car.py > /dev/tty.usbmodem1411 or 1421

************************
UPDATE Dec 2013

At Electric Imp hacakthon - reworked the car to feed commands through the imp

Hugo, Tom, Matt provided the guidance on how to write the imp code and pipe it from Leap to imp to Arduino.

Currently using CLI: python -u car.py | xargs -I % curl http://agent.electricimp.com/[address]?drivecommand=%

Basically car is now wireless

************************
Issue:
Latency in response using electric imp vs usb cord. Potentially due to wifi strength but this has happened with different wifi.
