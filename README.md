# brewAnywhere

This is not the offical Homebrew! OFFICAL:https://github.com/homebrew 

We're having a idea that a package manager should be portable. If you hava this idea too, try this!

## Few things to notice

Even though Homebrew says it would be buggy to build from source, but never be afraid, in most times, it won't fail! 

The Homebrew ENV file is on `${HOMEBREW_REPOSITORY}/Library/brew.env`, remember to leave a empty line in the end, because the last line won't be read. 

For the All In On Folder idea, we moved Caches and Logs directory to `${HOMEBREW_REPOSITORY}/Library` and moved "HOMEBREW_USER_CONFIG_HOME" to `${HOMEBREW_REPOSITORY}/Library/Config.d`

## A way to use packages outside current Homebrew

We had discovered a way to do this, though we're still not sure if it's a stable way. If you found any problem, report is here: https://github.com/brewAyW/brew/issues/4 

This would help a lot when you're having different brews around your system but don't want to build one same package again and again.

```
# First, the formula and version that match your outside package
mkdir [Homebrew Repository]/Cellar/[matched formula name]
ln -s Homebrew Repository]/Cellar/[matched formula name]/[matched version] [outside package's prefix]
# Finished!
```

Notice that you should first check if the outside package is the same to the Homebrew package (for example, Homebrew node.js and website downloaded node.js is different).

Suggestions: openssl is well needed and takes a long time to build. So try to link it!

## Installtion

```
git clone https://github.com/brewayw/brew [Homebrew Repository (Packages's Home)]
mkdir [Homebrew Prefix (like an interface)]
mkdir [Homebrew Prefix]/bin
ln -s [Homebrew Repository]/bin/brew [Homebrew Prefix]/bin/brew
```

# Homebrew

For more information, see the offical Homebrew README, https://github.com/homebrew/brew

Thank for all Homebrew contributers.