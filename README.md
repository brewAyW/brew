# brewAnywhere

This is not the offical Homebrew! OFFICAL:https://github.com/homebrew 

We're having a idea that a package manager should be portable and multi-user welcome. If you hava this idea too, try this!

## Few things to notice

Even though Homebrew says it would be buggy to build from source, but never be afraid, in most times, it won't fail! 

Sometimes Homebrew would suggest you to run a command, please look at the command carefully and DONT DO THAT IF IT'S FOR CHANGING PERMISSION! Just use ways you like to make that directory writable to you.

The Homebrew ENV file is on `${HOMEBREW_REPOSITORY}/Library/brew.env`, remember to leave a empty line in the end, because the last line won't be read. 

For the All In On Folder idea, we moved Caches and Logs directory to `${HOMEBREW_REPOSITORY}/Library` and moved "HOMEBREW_USER_CONFIG_HOME" to `${HOMEBREW_REPOSITORY}/Library/Config.d`

## Installtion

```
git clone -b master https://github.com/brewayw/brew [Homebrew Repository (Packages's Home)] --depth=1
mkdir [Homebrew Prefix (Packages' Interface)]
mkdir [Homebrew Prefix]/bin
ln -s [Homebrew Repository]/bin/brew [Homebrew Prefix]/bin/brew
```

## Developing Plans

- Because Homebrew Cask cannot support multi-user just by the way it work. So we are working on taking Homebrew Cask out of brewAnywhere.

- We also want to remove all the anti multi-user thing in brewAnywhere.

If you want to help, say in https://github.com/brewAyW/brew/issues/5.

# Homebrew

For more information, see the offical Homebrew README, https://github.com/homebrew/brew

Thank for all Homebrew contributers.
