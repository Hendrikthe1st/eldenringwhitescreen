# Elden Ring White Screen Crash
This is a small documentation in which I want to collect possible fixes for the white screen crash in elden ring.
Throughout this document I will discuss the fixes I personally came across and what I did to fix them.
When you want to add to this list or figure out what issue is the root of the problem i request you to search up the program "Reliability Monitor" click on your elden ring and check for the offset code.
The idea is to link the offset code for the crash to a fix, helping people with a more structored approach then current blogs are doing.

I want to shout out Dark Breed from Steam here, he helped me a lot throughout my process and is probably still working through steam threads as you read this.

<h1>Error Offset: 0000000000d431df</h1>
this error means there is something wrong with your Visual Redistributable C++. To fix this, look up "uninstall" and in the popup window look for Visual Redistributable C++, uninstall them and restart, then download the new ones:
https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170
after doing this restart again and it should be fixed

<h1>Error Offset: 0000000001e3e49d</h1>
I dreaded this one the most. This is an issue with your graphic drivers and is quite a doozy, check for the newest update on the website. DONT USE DEVICE MANAGER it wont find the update

<h2>Nvidia</h2>
For Nvidia use this website: https://www.nvidia.com/download/index.aspx
Make sure you take the correct one!
You can also use GeForce Experience to stay up to date.
If you have the newest update, use DDU to clean reinstall your nvidia drivers.

<h1>Error offset: 0x0000000001e576bb</h1>
This hints that you use Directx11 while the game needs Directx12, check if your pc is able to handle 12, because sometimes they wont despite advertised differently. If they cant I suggest refunding the game (sorry)

<h1>Error Offset something like: 000000000ffffff</h1>
the f's in this case are placeholders, as this is where my exact codes end. From here I will mostly add what dark breed told me:
"data and mostly caused by background apps that elevated apps to the wrong offset segment"
I heard some people struggle with epic games, i suggest trying after uninstalling it
You can also try to clean out your %temp% folder

<h1>Error Offset between: 000000000100000 to 000000000200000</h1>
Dark Breed: related to GPU driver and directx communications with the windows

<h1>Error Offset above: 000000000200000</h1>
Again for this segment i will quote dark breed as he has more insight in it then me:
"related to commnication between directx and GPU driver and the transport is made by the c++ library so any of this 3 parts can be involved into a crash there"

