# Changelog

## Unreleased

## Changed

+ relm4: Pass model in connect_components function of the Widgets trait
+ relm4: Added with_app method that allows passing an existing gtk::Appliaction to Relm4
+ book: Many book improvements by [tronta](https://github.com/tronta)

## Added

+ relm4: Re-export for gtk
+ relm4-macros: Allow usage of visibilities other than pub
+ relm4-macros: New pre_connect_components and post_connect_components for manuall components code

## Fixed

+ relm4-macros: [#20](https://github.com/AaronErhardt/relm4/issues/20) Fix wrong order when using components in the widget macro

## 0.1.0 - 2021-09-06

### Added

+ relm4: Added message handler type
+ relm4: More methods for factory data structures
+ relm4-macros: Add syntax for connecting events with components
+ relm4-examples: Stack example
+ book: Added macro expansion chapter

### Changed

+ book: Added message handler chapter and reworked the threads and async chapter
+ book: Many book improvements by [tronta](https://github.com/tronta)
+ relm4: The send! macro no longer clones the sender
+ relm4-macros: Make fields of public widgets public
+ relm4-components: Use &'static str instead of String for configurations
+ relm4-examples: Many improvements

### Fixed

+ relm4-macros: Use fully qualified syntax for factories
+ relm4-macros: Passing additional arguments now works for components and other properties, too.

## 0.1.0-beta.9 - 2021-08-24

## Added

+ relm4-components: Open button with automatic recent files list
+ relm4-components: Removed trait duplication and added more docs
+ relm4: Iterators added to factory data structures
+ relm4: More widgets added as FactoryView

### Changed

+ book: Many book improvements by [tronta](https://github.com/tronta)
+ relm4: Removed class name methods from WidgetPlus [#14](https://github.com/AaronErhardt/relm4/pull/14)

### Fixed

+ relm4-macros: Parsing additional fields should be more stable now
+ relm4-macros: Widgets can not include comments at the top 

## 0.1.0-beta.8 - 2021-08-20

### Added

+ relm4: Support for libadwaita 🎉
+ relm4-macros: Fully qualified syntax for trait disabiguation
+ relm4-macros: Allow passing additional arguments to widget initialization (useful e.g. for grids)
+ book: Reusable components and widget macro reference chapters

### Changed

+ relm4-macros: Improved error messages

## 0.1.0-beta.7 - 2021-08-19

### Added

+ book: Factory, components, worker and thread + async chapters

### Changed

+ relm4: get and get_mut of FactoryVec and FactoryVecDeque now return an Option to prevent panics

### Fixed

+ relm4-macros: Fixed components
+ relm4: Fixed unsound removal of elements in FactoryVecDeque


## 0.1.0-beta.6 - 2021-08-18

### Changed

+ relm4: Improved and adjusted the FactoryPrototype trait

### Added 

+ relm4: Added the FactoryListView trait for more flexibility
+ relm4: Added a FactoryVecDeque container
+ relm4: Implemented FactoryView and FactoryListView for more widgets
+ relm4-examples: More examples

### Fixed

+ relm4-macros: Fixed the factory! macro

## 0.1.0-beta.5 - 2021-08-15

### Added

+ relm4: Drawing handler for gtk::DrawingArea
+ relm4: New CSS methods in WidgetPlus trait
+ relm4-examples: Many new examples

### Changed

+ relm4: Many doc improvements
+ relm4-macros: Improved tracker! macro
