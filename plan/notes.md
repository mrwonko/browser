*   Maybe use the Chromium Embedded Framework?
    *   Either way use something that's faster than Firefox and displays pages properly.
    *   If I use Qt there's Qt WebEngine for embedded chromium
        *   Since I'd probably use Qt for the GUI anyway this is a natural choice
        *   Plus free mobile support!
*   organize tabs in a tree (think nested tab groups)
*   lazy loading of tabs (essential)
*   tabs double as favorites due to lazy loading and the tree-structure;
    in addition to closing there's also explicit unloading.
    *   any tab can get keywords/description; tab-switch can search those.
*   pinned tabs
*   session management could be done using the file system in a natural way - one file per website.
    *   filename: numeric, signifying order; contents: url (& possibly more in the future)
    *   this enables sharing and three-way merges using version control like git
        *   possibly directly support git, doing file management in a git-aware way
        *   although empty directories are not tracked by git
        *   in any case: **some kind of sync is desired**
    *   files could contain a GUID for better revision management
*   builtin password generator?
*   generalized commands (see: Vivaldi, Blender)
    *   Search field
    *   Keyboard shortcuts
*   smart address bar
    *   See [Mozilla's Frecency Algorithm](https://developer.mozilla.org/en-US/docs/Mozilla/Tech/Places/Frecency_algorithm) and [Slack's version thereof](https://slack.engineering/a-faster-smarter-quick-switcher-77cbc193cb60#.8rhnrjdq9)
