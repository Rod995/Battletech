# Rules

* Keep it to lore you demons.
* Custom Vehicles/BA/Mecha designs can only be from MegaMekLab or from Sarna.net.
* Tiles are considered 1.55 meters. Don't ask, it took a while. A long while.
* @Lord Rod, Lord of Rods [COM] for the vehicle speed rework, I approximated car width in meters as 0.4*tiles width  + 0.5 for tiles <= 5, 2.5 + ( tiles - 5 )*0.15m for larger
















































You want to know how I did it?
Here ya go.

Lord Rod, Lord of Rods [COM]Today at 4:33 PM
hm
ANFO is between a parcel and a car
You should run 150 feet away in a buildingto be safe.
100 feet must be dangerous then.
Soylent GrunToday at 4:34 PM
"/cygdrive/d/Cataclysm-DDA/src/ncurses_def.cpp:299: undefined reference to getch'" and "../cataclysm.a(debug.o):debug.cpp:(.rdata$.refptr._ZN10catacurses6stdscrE[.refptr._ZN10catacurses6stdscrE]+0x0): undefined reference tocatacurses::stdscr'
../cataclysm.a(ncurses_def.o): In function operator()':
/cygdrive/d/Cataclysm-DDA/src/ncurses_def.cpp:39: undefined reference todelwin'"
Lord Rod, Lord of Rods [COM]Today at 4:34 PM
oof
Soylent GrunToday at 4:36 PM
it is prob some sort of makefile error somewhere, but I have a lot of trouble reading makefiles
Lord Rod, Lord of Rods [COM]Today at 4:37 PM
also
Remind me to remove vehicle size limits.
Or extend them or something.
Soylent GrunToday at 4:37 PM
ow right, I wanted to test something else, runnign make tests inside the tests dir. See if that works
Lord Rod, Lord of Rods [COM]Today at 4:37 PM
b!remind bug kevin about size -t 1 day
BOT BOTBOTToday at 4:37 PM
 Ok! I'll remind you in a DM in a day! 
Soylent GrunToday at 4:38 PM
well that just gives all kinds of other errors. ../cataclysm.a(mondeath.o): In function _(char const*)':
/cygdrive/d/Cataclysm-DDA/src/translations.h:46: undefined reference tolibintl_gettext'
Prince SilvermaneToday at 4:38 PM
Changes to the C++ files can't be in .json format can they?  I was altering some values of nukes, mainly the radius.
Soylent GrunToday at 4:38 PM
no they can't 
Lord Rod, Lord of Rods [COM]Today at 4:38 PM
lol
Prince SilvermaneToday at 4:38 PM
Boo.
Lord Rod, Lord of Rods [COM]Today at 4:39 PM
+f
Nukes are hardcoded?
Prince SilvermaneToday at 4:39 PM
Not too familiar with .json but I know a bit about C++.  Good to know though.
Soylent GrunToday at 4:39 PM
C++ files need to be compiled by a compiler, the json files are interpreted by the program taht comes out of the compiler, sorry.
Prince SilvermaneToday at 4:39 PM
Yeah I found the radius in computer.cpp
Lord Rod, Lord of Rods [COM]Today at 4:39 PM
json ez pz
hm
Soylent GrunToday at 4:39 PM
json is simply put a way to write down data, it is like a comma seperated file, but human readable.
Lord Rod, Lord of Rods [COM]Today at 4:40 PM
Very readable
mlangsdorfToday at 4:40 PM
@Soylent Grun huh. yeah, okay, stop wasting your time. I'll pull your changes, run the efficiency tests, and put the results in the comments of your PR.
Soylent GrunToday at 4:40 PM
compared to a csv yeah.
Prince SilvermaneToday at 4:40 PM
Depending on your experience.
Lord Rod, Lord of Rods [COM]Today at 4:41 PM
wut I do @kybe
ah yes
Prince SilvermaneToday at 4:41 PM
I've fiddled with .json too, but I don't know what you can and can't do with them outside of using examples from other mods.
Lord Rod, Lord of Rods [COM]Today at 4:41 PM
Mapping extras did take 5 mins.
Soylent GrunToday at 4:42 PM
json files can also be ugly and hard to read btw
http://prntscr.com/l6v422
Lord Rod, Lord of Rods [COM]Today at 4:42 PM
LINT
Soylent GrunToday at 4:42 PM
(random .sav data)
Prince SilvermaneToday at 4:42 PM
If you don't open them in Notepad++
Oh yeah, .sav
That thing is a mess.
Lord Rod, Lord of Rods [COM]Today at 4:43 PM
+f
Prince SilvermaneToday at 4:43 PM
One of my saves are so big it breaks if I try to open it.
Soylent GrunToday at 4:45 PM
But lord, I simply downloaded astyle and put it in a directory and called that from a command line, didn't you get that to work?
Lord Rod, Lord of Rods [COM]Today at 4:45 PM
;w;
no know how to use
mlangsdorfToday at 4:46 PM
@Soylent Grun ran the tests for you, posted the results
Lord Rod, Lord of Rods [COM]Today at 4:46 PM
How do I tell it what files I wanna astyle?
Soylent GrunToday at 4:47 PM
let me check the astyle documentation, I always have to look it up.
Thanks @mlangsdorf
Lord Rod, Lord of Rods [COM]Today at 4:48 PM
Its sensitivity is relatively low; it generally requires a booster (e.g., one or two sticks of dynamite, as historically used, or, in more recent times, Tovex) to ensure reliable detonation. The explosive efficiency associated with ANFO is approximately 80% of TNT, also stated as TNT equivalency. 
hm
anfo needs dynamite
Call it Boosted ANFO....
lemme calculate TNT
20 pounds of nuclear thingie
coool
clarjon1Today at 4:49 PM
Looks like someone's having a blast.
Lord Rod, Lord of Rods [COM]Today at 4:50 PM
;w;
you demon
ugh
Gonna install an explosion simlutator.(edited)
Then gonna calculate ANFO using it...
I hope.
pfffft
Look at us.
Or them.
Cause I don't do bug fixes.
sigh
Installing VirtualBox
Soylent GrunToday at 4:59 PM
Righto, looked it up, you just need to install astyle (the binary, which is available on sourceforge for windows iirc) and then run <location of astyle for example ..\programs\astyle\bin\astyle.exe> --options=.astylerc <file you want to style for example 'src\player.cpp'>
Lord Rod, Lord of Rods [COM]Today at 4:59 PM
putting either ubuntu or linux mint on moi laptop again
Which one do you people prefer?
Soylent GrunToday at 5:00 PM
astyle then overwrites the cpp file with the styled one.
this is the unsafe way of course, you want a diff etc etc but if you just need to style your files quickly and know which ones, and have git installed etc you can quickly see changes.
Lord Rod, Lord of Rods [COM]Today at 5:05 PM
;w;
no loike this
i want moi simple linux
kinda simple linux
Soylent GrunToday at 5:05 PM
more info, and a prob safer way to do it https://github.com/CleverRaven/Cataclysm-DDA/blob/master/doc/CODE_STYLE.md
Lord Rod, Lord of Rods [COM]Today at 5:05 PM
Barely simple limux
;w;
how I use make again?
i cri
Soylent GrunToday at 5:09 PM
well make is easy just make make make 
make <target>
and the start of the makefile has some documentation.
(which a small error in it btw)
The error is that if you do TILES=0, there is still code that checks : ifdef TILES which messes things up
ralreegorganonToday at 5:11 PM
If you're on Windows 10 and don't mind docker, I have a docker image that will cross-compile for windows, and lets you run anything else you might normally run inside a CDDA compilation environment https://hub.docker.com/r/ralreegorganon/cddadockerwin/
Lord Rod, Lord of Rods [COM]Today at 5:12 PM
docker no work
Soylent GrunToday at 5:13 PM
I think it should be 'ifeq ($(TILES), 1)' not 'ifdef TILES' esp as there is documenation that tells you to do TILES=0.
prob easier to just edit the documentation in the places where it is wrong btw.
Lord Rod, Lord of Rods [COM]Today at 5:20 PM
all this work
for some explosions
