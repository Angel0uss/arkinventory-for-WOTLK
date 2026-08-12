General:

    * home page - http://arkinventory.googlecode.com/
	
	* faq - http://code.google.com/p/arkinventory/wiki/FAQ

	* betas;
		* backup your saved variables file for arkinventory
		* when installing a new beta always restore a copy of your saved variabes from the backup you made (so it's starts clean - theres usually no automatic upgrade between beta versions)

	* example rules - http://code.google.com/p/arkinventory/wiki/ExampleRules
	
	* download from;
		* google code - http://code.google.com/p/arkinventory/downloads/list
		* wow interface - http://www.wowinterface.com/downloads/info6488
		* curse gaming - http://wow.curse.com/downloads/wow-addons/details/ark-inventory.aspx
		* wow ui - http://wowui.worldofwar.net/?p=mod&m=4504
		
	* use WoW UI Updater to keep all your mods up to date - http://wuu.vagabonds.info/
	
	


Overview:

    * unlimited number of bars (there are practical limits though before your screen becomes full)
    * assign items to a category of your choice (overrides the default assignment)
    * assign categories to the bar of your choice
    * configurable bars per row
    * configurable width
    * display bank, bag, keyrings for current and alts across all realms
    * separate keybindings for bag, keyring and bank viewing
    * /arkinv ui reset (puts the windows back in the centre of the screen)
    * /arkinv db reset confirm (resets all user options back to defaults)
    * /arkinv cache erase confirm (erases all cached data - not options)
	
	* optimized - halved per-item scan cost by merging the soulbound/BoP tooltip check into a single pass instead of two
    * optimized - precomputed constant tooltip search patterns once instead of rebuilding them per item scanned
    * optimized - removed 5 duplicate closure allocations when summing bag counts
    * fixed - restack loop was re-querying bag slot count every iteration instead of once
    * added - Find Duplicates: menu action + Config -> Duplicates checkbox, fades everything except items split across 2+ separate slots, auto-clears on bag/bank close
    * added - "bag/slot position" is now a real, manageable sort criteria (previously a hidden fallback only)
    * added - per-criteria Reverse toggle in Sort Methods, each criteria now has its own independent direction instead of one global ascending/descending
    * fixed - vendor price sort could overflow on very high value stacks (widened padding)
    * added - "manual order" sort criteria: hand-arrange item order within a category via Edit Mode -> right-click item -> Move Left/Right
    * added - custom category display order: Config -> Categories -> pick a category -> Move Up/Move Down
    * added - Value Order: for Quality, Equip Slot, and Item Type sort criteria, an inline collapsible list to set the exact order of values (eg Head before Chest before Shoulder) via Up/Down buttons

	
	
	

	
Key Bindings (How To):

	Press ESCAPE to bring up the blizzard menu
	click on Key Bindings
	scroll down to ArkInventory
	bind the keys you want to use to specific functions
	
	
Issues:
	* the background can appear in front of the items rendering them unuseable - note this is not an ai code problem, it would appear to be an issue with blizzards CreateFrame api function.  a workaround for this issue is included in the addon config menu.


Bugs:
	* guild bank (vault) can have display issues on first open, just change tabs or refresh
	
	
To Do:


Version History:
	* see VersionHistory.txt or http://code.google.com/p/arkinventory/wiki/VersionHistory
