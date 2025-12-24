# FFXIV Crafting Macro Database

A web-based database for managing Final Fantasy XIV crafting macros and recipes

## Features

- **Craft Management**: Add, edit, and delete crafting recipes with detailed information
- **Macro Support**: Store macros with automatic splitting (15 lines per macro chunk)
- **Class Stats**: Configure and display class-specific stats (Craftsmanship, Control, CP)
- **Food & Potion Tracking**: Track required consumables for each craft
- **Search & Filter**: Find crafts by name or filter by class
- **Local Storage**: All data persists in your browser's localStorage
- **Copy to Clipboard**: Easy one-click copying of macros

## Craft Fields

Each craft entry includes:

- **Craft Name**: Unique identifier for the recipe
- **Craft Stats**: Level, Rating (1-4 stars), Durability, Difficulty, Quality
- **Food**: Optional checkbox with dropdown
- **Potion**: Optional checkbox with dropdown
- **Macro**: Multi-line macro text (auto-splits every 15 lines)
- **Class**: Select from 8 crafting classes
- **Notes**: Additional information or tips

## Classes

The following crafting classes are supported:

- Carpenter
- Alchemist
- Armorer
- Blacksmith
- Culinarian
- Goldsmith
- Leatherworker
- Weaver

Each class has configurable stats that display on all crafts using that class.

## Usage

### Adding a Craft

1. Click "Add Craft" button
2. Fill in the craft details
3. Optionally check "Requires Food" or "Requires Potion" and select from dropdown
4. Enter your macro (will automatically split into 15-line chunks)
5. Add notes if needed
6. Click "Add Craft" to save

### Managing Class Stats

1. Click "Manage Class Stats" button
2. Update Craftsmanship, Control, and CP for each class
3. Click "Save Stats"
4. These stats will automatically display on all crafts using each class

### Searching and Filtering

- Use the search box to find crafts by name
- Use the class dropdown to filter by specific classes

### Copying Macros

Each macro chunk has a "Copy" button that copies the macro text to your clipboard for easy pasting into FFXIV.

## Data Storage

All data is stored in your browser's localStorage:
- `craftingCrafts`: Array of all craft entries
- `craftingClassStats`: Object with stats for each class

**Note**: Clearing browser data will delete all stored crafts and stats. Consider exporting your data periodically (future feature).
