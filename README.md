# writing-tools

Just a collection of tools that I've asked Claude to build for me

The aim here is to build tools that fit my own, personal requirement.


### 1st one is a Character/Story mapper
Create a timeline of Events, Chapters, Dates etc
Add Characters to a list and place them on the timeline

Characters can be linked together in groups
Characters can be related to each other in any way you choose - e.g. Family, Crewmates, Allies, Enemies, etc
Add you characters where they come into the story and where they leave and how they related to others

Multiple timelines
Multiple characters per timelines
Multiple relationships

All running in pure html and javascript

Export your work to Mermaid diagrams, SVG, or text
Save you work as you go (JSON format) and import at a later date - work is also saved real time in the browser too

Everything can be run offline - but there is a github page to see it running live
https://netean.github.io/writing-tools/Story%20Character%20Mapper.html

#### Text Export Example
When you ask for an output in text you get an outline and overview

```
The Lighthouse Keepers
======================
Exported 31/10/2026, 16:55:52

CHARACTERS
----------
• Mara Vell
  Groups: Keepers
  In "Book I — The Lamp": Arrival – Salvage (The Harbour); Night watch – Return (The Island)
    ← Old Fenn · Family · from Arrival onward
    → Lio · Family · from The storm onward
    → Iris Kade · Romance · from Lamp fails onward
  In "Book II — Charts": May 1892 – Aug 1892 (Main thread)
• Tobin Ash
  Groups: Crew of the Ostra
  In "Book I — The Lamp": Salvage (The Island); The crossing – Return (The Harbour)
    ← Captain Rhee · Ally · from Salvage onward
    → Iris Kade · Rival · from Wreck found until The crossing
• Iris Kade
  In "Book I — The Lamp": Wreck found – The crossing (The Island)
    ← Tobin Ash · Rival · from Wreck found until The crossing
    ← Mara Vell · Romance · from Lamp fails onward
  In "Book II — Charts": Jul 1892 – Oct 1892 (Main thread)
    ← Old Fenn · Ally · from Jul 1892 onward
• Old Fenn
  Groups: Keepers
  In "Book I — The Lamp": Arrival (The Harbour); Lamp fails (The Harbour)
    → Mara Vell · Family · from Arrival onward
  In "Book II — Charts": Jun 1892 – Jul 1892 (Lane 2)
    → Iris Kade · Ally · from Jul 1892 onward
• Captain Rhee
  Groups: Crew of the Ostra
  In "Book I — The Lamp": The storm – Night watch (The Island)
    → Tobin Ash · Ally · from Salvage onward
• Lio
  Groups: Keepers
  In "Book I — The Lamp": The storm – Wreck found (The Harbour)
    ← Mara Vell · Family · from The storm onward

GROUPS
------
• Keepers: Mara Vell, Old Fenn, Lio
• Crew of the Ostra: Captain Rhee, Tobin Ash

RELATIONSHIP TYPES
------------------
• Family
• Ally
• Rival
• Romance

STORY: BOOK I — THE LAMP
------------------------
Axis: Chapters, 8 steps
  1. Arrival
  2. The storm
  3. Salvage
  4. Wreck found
  5. Night watch
  6. Lamp fails
  7. The crossing
  8. Return

Events:
  • Storm hits (at The storm)
  • Ostra sinks (at Wreck found)
  • Fenn falls (at Lamp fails)

Date markers:
  • Autumn 1891 (at Arrival)
  • Winter (at Night watch)

Timeline by lane:
  The Harbour
    • Mara Vell: Arrival – Salvage
    • Old Fenn: Arrival
    • Lio: The storm – Wreck found
    • Old Fenn: Lamp fails
    • Tobin Ash: The crossing – Return
  The Island
    • Captain Rhee: The storm – Night watch
    • Tobin Ash: Salvage
    • Iris Kade: Wreck found – The crossing
    • Mara Vell: Night watch – Return

Relationships:
  • Old Fenn → Mara Vell · Family · from Arrival onward
  • Mara Vell → Lio · Family · from The storm onward
  • Captain Rhee → Tobin Ash · Ally · from Salvage onward
  • Tobin Ash → Iris Kade · Rival · from Wreck found until The crossing
  • Mara Vell → Iris Kade · Romance · from Lamp fails onward

STORY: BOOK II — CHARTS
-----------------------
Axis: Dates (1892-05-01 to 1892-12-31, by month), 8 steps
  1. May 1892
  2. Jun 1892
  3. Jul 1892
  4. Aug 1892
  5. Sept 1892
  6. Oct 1892
  7. Nov 1892
  8. Dec 1892

Chapters:
  • Chapter 1 (at May 1892)
  • Chapter 2 (at Jun 1892)
  • Chapter 3 (at Jul 1892)
  • Chapter 4 (at Aug 1892)
  • Chapter 5 (at Sept 1892)
  • Chapter 6 (at Oct 1892)

Timeline by lane:
  Main thread
    • Mara Vell: May 1892 – Aug 1892
    • Iris Kade: Jul 1892 – Oct 1892
  Lane 2
    • Old Fenn: Jun 1892 – Jul 1892
  Lane 3
    (empty)
```

Relationships:
  • Old Fenn → Iris Kade · Ally · from Jul 1892 onward
