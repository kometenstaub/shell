# Shell scripts

This is a collection of shell scripts.

**Please, have backups and try out the script(s) in a test vault first!**

Should you find any bugs, please open an issue.

## update_plugin

This script is meant to facilitate updating plugins which are not in the Obsidian community plugin store. The developer might not have submitted the plugin or it is still in development before it is submitted.

I created the script to make being a plugin beta tester easier. Currently, I have only tested it with the plugin you can find under the sample URL.

It downloads the latest release.

See the comments for more details.

You may have to adjust the code slightly for the plugin you want to use it with.

## vault_search

This script is a first try at making a shell script that searches a note in your Obsidian vault for links and appends text to these linked notes.

### Usage

You need to change `vaultPath` inside the script and have `ripgrep` and `fd` installed.

Execute the script like this:

`./vault_search 'name of the note' 'text to append'`

Specify `name of the note` without the `.md` extension. If it is the only note with this name in your vault, just specify the name, you don't need to specify the path from the vault root. 

The text you want to append cannot include `\n` as new line character.


