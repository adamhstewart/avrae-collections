# Arrow Alias

A unified alias for making attacks with different magical arrow types.

**Features:**
- Supports multiple arrow types: magefire, ice
- Automatically tracks ammunition using custom counters
- Handles weapon attacks with special arrow effects
- Optional target specification
- Automatic save DC calculation for ice arrows

**Arrow Types:**
- **Magefire**: Adds 1d6 fire damage, arrows consumed on use
- **Ice**: Sets damage to 0, forces Constitution save (DC = 8 + prof + attack stat) for movement reduction

**Setup:**
Create counters for each arrow type you want to use:
- `!cc create "Magefire Arrows" -max <amount>`
- `!cc create "Ice Arrows" -max <amount>`

**Usage:**
```
!arrow <weapon> <arrow_type> [-t <target>]
```

**Examples:**
- `!arrow longbow magefire -t goblin`
- `!arrow "shortbow +1" ice -t "orc warrior"`
- `!arrow crossbow magefire`

**Parameters:**
- `<weapon>`: Name of the weapon to attack with
- `<arrow_type>`: Type of arrow (magefire, ice)
- `-t <target>`: Optional target name

The alias will automatically execute the appropriate attack command with the arrow's special effects applied.