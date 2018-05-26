
# Webtrees Custom Module: ⚶ Gov4Webtrees

This [webtrees](https://www.webtrees.net/) custom module hooks into an extended 'Facts and Events' tab, enhancing events with [GOV](http://gov.genealogy.net) (historic gazetteer) data.
The project’s website is [cissee.de](https://cissee.de).

## Contents

* [Features](#features)
* [Demo](#demo)
* [Download](#download)
* [Installation](#installation)
* [License](#license)

### Features<a name="features"/>

* Historic and current GOV data is loaded, cached internally, and displayed for individual events. Map links (to OpenStreetMaps etc) based on geodata obtained from the GOV server are also shown.

![GOV](GOV.png)
* GOV ids have to be entered manually, once per place name. Alternatively, ids for specific events may be set via a custom _GOV tag under the respective PLAC tag.

### Demo<a name="demo"/>

Access a demo of the module [here](https://cissee.de/gov4webtreesDemo). Feel free to experiment with setting/resetting GOV Ids.

### Download<a name="download"/>

* Current version: 1.7.9.14
* Based on and tested with webtrees 1.7.9, may also work with older 1.7.x versions.
* Requires the Hooks module ('hooks_repackaged', or the original Hooks module via webtrees-geneajaubart). 
* Requires the 'vesta_common_lib' module.
* Displays data via the 'personal_facts_with_hooks' module.
* Provides location data via hooks.
* Download the zipped module, including all related modules, [here](https://cissee.de/vesta.latest.zip).
* Support, suggestions, feature requests: <ric@richard-cissee.de>
* Issues also via <https://github.com/ric2016/gov4webtrees/issues>
 
### Installation<a name="installation"/>

* Unzip the files and copy them to the modules_v3 folder of your webtrees installation. All related modules are included in the zip file. It's safe to overwrite the respective directories if they already exist (they are bundled with other custom modules as well), as long as other custom models using these dependencies are also upgraded to their respective latest versions.
* Enable the extended 'Facts and Events' module via Control Panel -> Modules -> Module Administration -> Facts and Events.
* Enable the main module via Control Panel -> Modules -> Module Administration -> Gov4Webtrees. After that, you may configure some options.
* Enable the Hooks module via Control Panel -> Modules -> Module Administration -> Hooks. Make sure all hooks are selected (in the preferences of the Hooks module).				
* Configure the visibility of the old and the extended 'Facts and Events' tab via Control Panel -> Modules -> Tabs (they both appear as 'Facts and Events' here - usually, you'll want to use only one of them. You may just disable the old 'Facts and Events' module altogether).
				
#### Import/Export

If you want to transfer GOV data between different trees or webtrees instances, you only have to copy the table which maps place names to gov ids (##gov_ids), everything else will be re-created automatically.
If you use GEDCOM data with _GOV tags for GOV ids, even this step is unnecessary.


### License<a name="license"/>

* **gov4webtrees: a webtrees custom module**
* Copyright (C) 2016 to 2018 Richard Cissée
* Derived from **webtrees** - Copyright (C) 2010 to 2016  webtrees development team.
* Derived from **webtrees-geneajaubart** - Copyright (C) 2009 to 2016  Jonathan Jaubart.
* Nutzt Daten des [Geschichtlichen Ortsverzeichnisses GOV](http://gov.genealogy.net) des [Vereins für Computergenealogie e. V.](http://compgen.de).

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.

