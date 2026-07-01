# Stellaris: Unlock Portrait Traits!

This is a simple Stellaris mod that removes portrait-based restrictions on various species traits.
For example, the "Flying" trait no longer requires an Avian portrait, or one of the specially-excepted flying lizard or insect portraits;
the "Scintillating" trait no longer requires a Lithoid portrait;
etc.

Unlike several other trait-unlocking mods, this *does not* unlock *every* trait;
there are a whole lot of event/origin/etc-locked traits that are not intended or balanced for species creation.
It just unlocks the existing traits that are available at species creation,
but locked behind a particular species category or portrait.
(This also means your trait list isn't *enormously* expanded, just a bit from core.)

* Machine/Robotic vs Bio/Lithoid restrictions are still maintained, as those generally make sense.
* Same with Nomadic restrictions.
* This mod *correctly* unlocks Tankbound; some other mods that purport to do so break Tankbound empires because they don't adjust the Tankbound civic too.

----------

Touched files:

* `common/governments/civics/00_civics.txt` - for Tankbound
* `common/traits/04_species_traits.txt` - for Lithoid/Plantoid-only traits
* `common/traits/15_biogenesis_species_traits.txt` - a *whole bunch* of traits
* `common/traits/16_infernals_traits.txt` - for Infernal-only traits
* `common/traits/17_shroud_species_traits.txt` - for Psionic-only traits, and Tankbound

Any other mod which touches these files will conflict,
even if it only touches traits that never cared about the portraits in the first place.
Unfortunately, the way traits are loaded means I can't limit my effects to just the relevant traits;
I have to override the whole file.

If you don't care about unlocking the categories of traits that are in the conflicting files,
feel free to put this mod earlier in the load order,
so the conflicting mod wins.

Maintained in the Steam Workshop at <https://steamcommunity.com/sharedfiles/filedetails/?id=3686317383>
