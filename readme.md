# fan87's Regex Cheatsheet Collection

A cheatsheet that contains most complicated regex I've ever used in my life.



## File name format

The format should looks something like this: `(<?Languages>(?<Language>[\w\n\s]*)[1,]-)?(?<Name>[\w\n\s])(-(?<Sub name>[\w\n\s]))\.md`, or more human readable format: `<Language>?-<Name>-<Sub name>?`.

The language is the language that can be used on, name is the short description of it, and sub name is literally the sub name.

For example: `Java-Delegation` means that it can be used in a Java IDE on Java, and using it can make delegation classes quickly.

## Phases

If a regex has multiple phases, you need to replace them for multiple times (Because regex still has a limit).

## Human Readability

I don't think regex are created to be human readable (Comments and indent are not supported), so don't worry if you are lazy to understand or read them. Well you can still try but it's not worth it unless you are still learning regex.