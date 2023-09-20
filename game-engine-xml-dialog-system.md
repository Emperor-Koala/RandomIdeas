# Game Engine XML Dialog System

The idea is to create a library for a game engine (or even just a programming language like Java) that allows reading XML files as a "script" for dialog. These XML files could use tags to denote different stylings/effects.

By default, the library would incldue the following tags:
* `<line>` - Indicates one line of dialog
* `<bold>` - Indicates that the contained text should be **bold**
* `<italics>` - Indicates that the contained text should be *italics*
* `<font name="">` - Indicates the contained text should be a specific font

The library should also allow for new tags to be defined on the fly. For example, one could define a `<glitch>` tag that could trigger an effect of typing the text, then briefly "glitch" to show another text, possibly with different styling.