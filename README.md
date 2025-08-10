# Custom TTRPG System for Foundry VTT

A professional modular TTRPG system with advanced UI features, class progression, and MMO-style equipment management.

## 🚀 Current Status: 0.0.1 (Baseline)

**Version:** 0.0.1  
**Repository:** Successfully connected to GitHub  
**Status:** All files validated and ready for Foundry VTT installation

## ✨ Features

### Core Features
- ✅ Editable character sheets with dynamic attributes
- ✅ Class-based progression system (Monk, Warlock, Wizard, Fighter)
- ✅ Resource management (HP, Mana, Stamina, etc.)
- ✅ Inventory and spell management
- ✅ Combat tracking and feat system

### Advanced Features (0.0.1)
- ✅ **Equipment Manager**: MMO-style equipment interface
  - 16 equipment slots (head, neck, shoulders, etc.)
  - Drag and drop functionality
  - Real-time stat calculations
  - Item browser with search

- ✅ **Abilities Manager**: Class-specific abilities and features
  - Resource trackers (Ki Points, Pact Magic, etc.)
  - Class features (Monk auras, Warlock pacts, etc.)
  - Ability cooldowns and effects
  - Category-based organization

- ✅ **Compendium Manager**: Game content browser
  - Search and filter items, spells, abilities
  - Export/import functionality
  - Categorized content management
  - Add directly to character Inventory/Spells/Abilities

### Sheet & Apps
- ✅ Character sheet: Equipment, Abilities, Feats, Inventory, Combat
- ✅ Equipment slots with set bonuses, loadouts, preferred gear
- ✅ Abilities quick-use with costs/cooldowns and macros
- ✅ Feats enable/disable with live bonuses and macros
- ✅ Styled chat cards for Attack/Damage
- ✅ Combat Tracker: token import, actor link, quick rolls, HP sync
- ✅ Inventory Manager: double-click equip/unequip; overweight warning

## 🛠️ Installation

### Quick Install (Windows)
1. Copy this project folder to your Foundry Data `systems` directory and name it `custom-ttrpg`
2. Launch Foundry VTT and enable the system

### Manual Install
1. Copy this entire folder to your Foundry VTT `systems` directory
2. Rename the folder to `custom-ttrpg`
3. Start Foundry VTT and enable the system

## 🧪 Testing

### System Validation
Run `test-system.js` to validate the system structure:
```bash
node test-system.js
```

### Foundry VTT Testing Checklist
- [ ] System appears in Foundry VTT module list
- [ ] Can create new characters
- [ ] Character sheet displays properly
- [ ] Equipment Manager opens without errors
- [ ] Abilities Manager opens without errors
- [ ] Compendium Manager opens without errors
- [ ] Drag and drop works in Equipment Manager
- [ ] Resource trackers update correctly
- [ ] No JavaScript errors in console

## 📁 File Structure

```
custom-ttrpg/
├── system.json                    # System configuration
├── module/
│   ├── init.js                   # Main initialization
│   ├── class-loader.js           # Class data loader
│   ├── compendium-loader.js      # Compendium data manager
│   ├── applications/
│   │   ├── equipment-manager.js  # MMO-style equipment UI
│   │   ├── abilities-manager.js  # Class abilities and features
│   │   ├── compendium-manager.js # Content browser
│   │   └── ...                   # Other applications
│   └── sheets/
│       └── character-sheet.js    # Character sheet logic
├── templates/
│   ├── actors/
│   │   └── character-sheet.html  # Main character sheet
│   └── applications/
│       ├── equipment-manager.html
│       ├── abilities-manager.html
│       └── compendium-manager.html
├── styles/
│   └── custom-ttrpg.css         # System styling
└── data/
    ├── Classinfo.json            # Class definitions
    └── compendium.json           # Game content
```

## 🔧 Development

### Key Components
- **ES6 Modules**: Modern JavaScript module system
- **Handlebars.js**: Dynamic HTML templating
- **Foundry VTT Hooks**: Lifecycle management
- **Drag & Drop**: Equipment system integration
- **Resource Tracking**: Class-specific features

### Debug Commands
In Foundry VTT browser console (F12):
```javascript
// Check system loading
console.log(game.system.id); // Should return "custom-ttrpg"

// Check registered applications
console.log(CONFIG.CustomTTRPG);

// Test class data
console.log(CONFIG.CustomTTRPG.ClassInfo);
```

## 🐛 Troubleshooting

### Common Issues
1. **System Not Appearing**: Check folder name is `custom-ttrpg`
2. **JavaScript Errors**: Check browser console (F12)
3. **Template Errors**: Verify all HTML files exist
4. **Module Import Errors**: Check ES6 syntax

### Error Reporting
If you encounter issues:
1. Check the browser console (F12)
2. Note any error messages
3. Test with different character classes
4. Report specific error details

## 📈 Next Steps

After successful installation:
1. **Test All Features**: Try equipment, abilities, and compendium managers
2. **Performance Check**: Monitor for lag or slow loading
3. **Class Testing**: Test with different character classes
4. **UI Feedback**: Note any usability improvements needed

## 📄 License

MIT License - See LICENSE.md for details

## 🤝 Contributing

This system is actively developed. Report issues and feature requests through GitHub.

---

**Status:** ✅ Ready for Foundry VTT testing  
**Last Updated:** Current session  
**GitHub:** https://github.com/browneas0/Custom-ttrpg-V2.git
