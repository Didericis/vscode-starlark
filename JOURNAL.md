# [Starlark VSCode Language Support Journal](diurnum://new?type=journal)

## 2024-06-22 10:54

This project started like [this lightbulb changing scene](https://www.youtube.com/watch?v=AbSehcT19u0):

- Saw that my [tidbyt](https://tidbyt.com/) said "Airthings Credential Missing" for my airthings app
- Tried to remember how tidbyt worked/how I could push code up
- Went into a repo for a sample project I remember pushing to my tidbyt
- Saw that there wasn't any syntax highlighting for the "star" file
- Looked for an extension, only one I found has 1.5 stars and people saying it doesn't work (and I vaguely remember it not working)
- Started following instructions mentioned in [this blog post](https://mathspp.com/blog/til/vscode-extension-for-custom-syntax-highlighting) for creating syntax highlighting
- Saw that there was a "language support" option in the yeoman code generator
- Looked up what that was, read up on [the language server extension guide](https://code.visualstudio.com/api/language-extensions/language-server-extension-guide)
- Decided why not try and make one in an hour/see what happens

## 2024-06-22 11:12

Found a starlark grammar in [this repo](https://github.com/bazelbuild/vscode-bazel). That should allow me to do syntax highlighting. Specific location of the grammar was found [here](https://github.com/bazelbuild/vscode-bazel/blob//0.10.0/syntaxes/starlark.tmLanguage.json).

## 2024-06-22 11:22

Found starlark language configuration [here](https://github.com/bazelbuild/vscode-bazel/blob//0.10.0/syntaxes/starlark.configuration.json).

## 2024-06-22 11:25

I should probably reduce the scope of this/just make it syntax highlighting rather than getting into the full weeds of language support stuff. Don't think I need it. Plus I'm not sure exactly how to run starlark for tidbyt/would have to do a refresher.

## 2024-06-22 12:13

Got sucked down a bit of a license rabbit hole, but only a couple minutes over the timebox. Success!