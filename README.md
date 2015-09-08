# zsh-xcode-completions

Zsh completions for some of the Xcode command line tools. Currently:

- [`genstrings`](https://developer.apple.com/library/mac/documentation/Darwin/Reference/ManPages/man1/genstrings.1.html)
- [`nm`](https://developer.apple.com/library/mac/documentation/Darwin/Reference/ManPages/man1/nm.1.html)
- [`xcode`-select](https://developer.apple.com/library/mac/documentation/Darwin/Reference/ManPages/man1/xcode-select.1.html)
- [`xcodebuild`](https://developer.apple.com/library/mac/documentation/Darwin/Reference/ManPages/man1/xcodebuild.1.html)
- [`xcrun`](https://developer.apple.com/library/mac/documentation/Darwin/Reference/ManPages/man1/xcrun.1.html) See [shims](#shims) for more info
- `strings`
- `swift`
- `swift`-demangle

# Installation

```sh
brew install keith/formulae/zsh-xcode-completions
```

# TODO:

- lipo
- otool
- pkgutil

### Shims

Unfortunately, because of how `xcrun` happens to work, creating
completions that also handle the nested completions for programs run
through `xcrun` (such as `swift-demangle`) has proven to be difficult.
To get around this, I have created [shims](bin) for programs that could
use completions. I've also added a homebrew option (`--without-shims`)
if you would like to exclude these from being installed. One
disadvantage to this approach is you cannot pass arguments to the
`xcrun` command while calling a shim.

### Resources

<https://github.com/zsh-users/zsh-completions/blob/master/zsh-completions-howto.org>
