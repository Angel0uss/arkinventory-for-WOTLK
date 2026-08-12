# 3.1 (08-11-2026)

*custom build 3.1 (Angelouss, on top of 3.02.54 BETA 17-00-Cataclysm)*


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

