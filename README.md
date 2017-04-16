# nsL Assembler for Atom

[![apm](https://img.shields.io/apm/l/language-nsl.svg?style=flat-square)](https://atom.io/packages/language-nsl)
[![apm](https://img.shields.io/apm/v/language-nsl.svg?style=flat-square)](https://atom.io/packages/language-nsl)
[![apm](https://img.shields.io/apm/dm/language-nsl.svg?style=flat-square)](https://atom.io/packages/language-nsl)
[![Travis](https://img.shields.io/travis/idleberg/atom-language-nsl.svg?style=flat-square)](https://travis-ci.org/idleberg/atom-language-nsl)
[![David](https://img.shields.io/david/dev/idleberg/atom-language-nsl.svg?style=flat-square)](https://david-dm.org/idleberg/atom-language-nsl?type=dev)
[![Gitter](https://img.shields.io/badge/chat-Gitter-ed1965.svg?style=flat-square)](https://gitter.im/NSIS-Dev/Atom)

Atom language support for [nsL Assembler](https://sourceforge.net/projects/nslassembler/), including grammar, snippets and build system

![Screenshot](https://raw.github.com/idleberg/atom-language-nsl/master/screenshot.png)

*Screenshot of nsL Assembler in Atom with [Hopscotch](https://atom.io/themes/hopscotch) theme*

## Installation

### apm

* Install package `apm install language-nsl` (or use the GUI)

### Using Git

Change to your Atom packages directory:

```bash
# Windows
$ cd %USERPROFILE%\.atom\packages

# Linux & macOS
$ cd ~/.atom/packages/
```

Clone repository as `language-nsl`:

```bash
$ git clone https://github.com/idleberg/atom-language-nsl language-nsl
```

### Package Dependencies

This package automatically installs third-party packages it depends on. You can prevent this by disabling the *Manage Dependencies* option in the package settings.

## Usage

### Building

As of recently, this package contains a build system to translate nsL code into NSIS script and transpile it. To do so, select *Nsl Assembler: Save & Transpile”* from the [command-palette](https://atom.io/docs/latest/getting-started-atom-basics#command-palette) or use the keyboard shortcut.

Make sure to specify the path for `nsL.jar` in the package settings. There you can also customize the flags for the transpiler.

**Example:**

```cson
"language-nsl":
  pathToJar: ""%PROGRAMFILES%\\NSIS\\NSL\\nsL.jar"
  customArguments: "/nopause /nomake"
```

#### Third-party packages

Should you already use the [build](https://atom.io/packages/build) package, you can install the [build-nsl](https://atom.io/packages/build-nsl) provider to build your code.

## License

This work is dual-licensed under [The MIT License](https://opensource.org/licenses/MIT) and the [GNU General Public License, version 2.0](https://opensource.org/licenses/GPL-2.0)

## Donate

You are welcome support this project using [Flattr](https://flattr.com/submit/auto?user_id=idleberg&url=https://github.com/idleberg/atom-language-nsl) or Bitcoin `17CXJuPsmhuTzFV2k4RKYwpEHVjskJktRd`