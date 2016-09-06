# Base xcconfigs

Using xcconfigs, instead of modifying settings in an Xcode project, is my preferred way of configuring targets. They allow for reuse of settings across projects and targets. They also allow for standardization of settings for specific types of targets (eg. iOS app, tvOS app, Universal framework), which is the purpose of this repository.

By using the xcconfigs in this repository as a basis for your own xcconfigs (either via `#include` or copying) you should achieve a solid foundation for your project's and target's settings. The xcconfigs use a hierarchical structure to allow for easy maintainability.

## Target Configurations

For target level configurations there are the following base xcconfigs:

- Applications
    - iOS, Mac OS X, tvOS, and watchOS
- Extensions
    - iOS, Mac OS X, tvOS, and watchOS
- Frameworks
    - iOS, Mac OS X, tvOS, watchOS, and Universal
- Tests
    - iOS, Mac OS X, tvOS, and Universal
    - _watchOS currently doesn't support tests_

_Note:_ "Universal" above means having a single target that can compile for any of the other listed platforms.

## Project Configurations

For project level configurations there are the following base xcconfigs:

- Debug
- Release

## Usage

TODO _(Recommend submodule for integration. Describe normal `#include` usage. Describe normal project group setup for selection by Xcode.)_

## Credits

Inspired by [@jspahrsummers's](https://github.com/jspahrsummers/xcconfigs/pull/43) and [@mrackwitz's](https://github.com/mrackwitz/xcconfigs) xcconfigs.  
[@samdmarshall's](https://github.com/samdmarshall) [unofficial guide to xcconfig files](http://pewpewthespells.com/blog/xcconfig_guide.html) was also very helpful.
