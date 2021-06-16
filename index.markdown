---
layout: page
title:  The West Marches of Groton
permalink: /
---

# Players
<ul>
{% assign sorted_names = site.data.players | sort: "name" %}
{% for member in sorted_names %}
  <li>
    {{ member.name}}
    {% assign characters = site.data.characters | where: "player", member.name %}
    <ul>
    {% for character in characters %}
      <li>
      <a href="{{character.dndbeyond}}">{{character.character}}</a> Level: {{character.level}}
    </li>
    {% endfor %}
    </ul>
  </li>
{% endfor %}
</ul>

# Links
* The campaign in [DND Beyond][dnd_beyond]
* [The character building document][character_builder]
* [The Spreadsheet tracker][spreadsheet_tracker]
* [Darker Dungeons][darker_dungeons]
* [Session Reports][session_reports]

What is a [West Marches Campaign][west_marches_stackexchange]?

Going off of that, we have a fairly fixed time on Wednesday nights. However, anyone may attend and use any active character they 
own, or roll up a new one.  Players are encouraged to have multiple PC's.

Each session will begin and end in town.  The characters might not actually get back to town during the play session, but it
is assumed to happen.  Note, in certain circumstances, the route back to town might not be safe.  The worst that will happen is that 
the characters will be "lost" and not available for the next session(s).  Fire up a new character until the old one wanders back
into town.

[west_marches_stackexchange]: https://rpg.stackexchange.com/questions/120770/what-defines-a-west-marches-campaign
[dnd_beyond]: https://www.dndbeyond.com/campaigns/1993550
[character_builder]: https://docs.google.com/spreadsheets/d/1gsH4J1rAXI_LUvaBDZAmiqRY5wA3El9pA_nQaIqzdz8/edit#gid=0
[spreadsheet_tracker]: https://docs.google.com/spreadsheets/d/1qtLf07onMcsfyJLDcySESCcGAodHCR0pUAa0RWyz5G0/edit#gid=1056829732
[darker_dungeons]: https://giffyglyph.com/darkerdungeons/grimoire/3.1.1/en/
[session_reports]: /sessions
