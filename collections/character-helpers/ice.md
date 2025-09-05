# Ice Arrows

A snippet for tracking magical ammunition that removes base damage but forces a Constitution save to reduce target movement.

**Features:**
- Tracks remaining Ice Arrows using custom counters
- Removes base attack damage on hit
- Forces Constitution save (DC = 8 + proficiency bonus + attack stat)
- On failed save: target's movement reduced by 10 feet until end of attacker's next turn
- Arrows are consumed on use (cannot be recovered)
- Requires manual counter creation with desired amount

**Mechanics:**
- Uses Dexterity modifier for ranged attacks by default
- Falls back to Strength modifier if attack stat is set to strength
- Save DC automatically calculated based on attacker's stats

**Setup:** 
Create a counter first: `!cc create "Ice Arrows" -max <amount>`

**Usage:** 
Use this snippet when making ranged attacks with Ice Arrows to automatically track ammunition and apply the ice effect.