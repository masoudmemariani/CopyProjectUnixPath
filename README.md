# Copy Project Unix Path
A very simple extension for Visual Studio made out of frustration over a narrow case:

For using .NET CLI in a Git Bash inside Windows Terminal on Windows, I need to `cd` to the project's directory to build, run, etc. The context menu in Visual Studio's solution explorer gives me the full path to the project in the Windows format i.e. with backslashes as the path delimiter while Git Bash needs the Unix/Linux style i.e. with forward slashes. To convert the baclslashes to forward slahses in the path you can use the bash commands:

```console
$ t='\a\b\c'
$ echo "${t//\\//}"
```

But it's an extra step and why not using fewer clicks and keystrokes? By using this extension you can get the path to the project directory copied to your clipboard so that in Git Bash you can just `cd ctrl+v`.



