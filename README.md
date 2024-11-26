# A visual C# EditorConfig generator

## Background & Overview
**What is EditorConfig?**
> EditorConfig helps maintain consistent coding styles for multiple developers working on the same project across various editors and IDEs. The EditorConfig project consists of a file format for defining coding styles and a collection of text editor plugins that enable editors to read the file format and adhere to defined styles. EditorConfig files are easily readable and they work nicely with version control systems.
> https://editorconfig.org/

There are multiple C#/.NET code style rules that can be expressed in an `.editorconfig` file (see [this documentation](https://learn.microsoft.com/en-us/dotnet/fundamentals/code-analysis/code-style-rule-options#example-editorconfig-file)), such as indentation, parenthesis style, initializer style, namespace style, etc. etc.

What I want is a web-based tool for a team to collaboratively and visually explore these different style options, with clear examples, and then pick which one they prefer. Once you are done you get a generated `.editorconfig` file that represents the choices you've made that you can import directly into your project/repo and start using.
 
## Features
- Web-based tool
- Potentially a "Tinder-like" UI where you swipe left or right on different rules
- Simple and minimal UI, playful
- You should be able to pick which different rule categories you are intested in before you begin, so as to not overwhelm the user
  - For example:
    - [ ] *Naming rules*
    - [ ] *Naming styles*
    - [ ] *New line preferences*
    - [ ] Etc.
    - [ ] Or *All rules*
  - Any category you don't pick should use the default options for those rules

## Tech stack
- .NET 9/10
- React?
- Docker
- Azure?

## Other examples
The idea is very similar to this project that I found:
- https://github.com/KristofferStrube/EditorConfigWizard
- https://kristofferstrube.github.io/EditorConfigWizard/wizard

but (a) the site is pretty basic and ugly, (b) it doesn't do everything I want it to do, and (c) the project seems largey abandoned since march 2023.

## Links
- https://editorconfig.org/
- https://learn.microsoft.com/en-us/dotnet/fundamentals/code-analysis/code-style-rule-options
- https://learn.microsoft.com/en-us/visualstudio/ide/create-portable-custom-editor-options?view=vs-2022

### EditorConfig examples
- https://github.com/dotnet/razor/blob/main/.editorconfig
- https://github.com/dotnet/roslyn/blob/main/.editorconfig
- https://gist.github.com/RealDotNetDave/dbae4d97358ba4515dd52e5b8ca87671
- https://learn.microsoft.com/en-us/dotnet/fundamentals/code-analysis/code-style-rule-options#example-editorconfig-file
