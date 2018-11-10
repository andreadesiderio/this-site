# Syna Start

This is a sample project that can be used to jump start your Syna project. It uses Syna theme and Hugo with sample files that introduce two simple pages, one for landing and one for the about page.

## Installation

To start using this starter you need to download this repository and update it's git submodules (Syna theme is added as a submodule).

```
git clone git@github.com:okkur/syna-start.git project-name && cd $_
git submodule init
git submodule update
```

## Usage

To start your blog run the following commands:

**Development**:
```
$ hugo server -D
```

**Production**:
```
$ hugo # This command would generate the static website in the public directory
```

> Prerequisites: Go, Hugo

## Directory Structure

We're using the standard directory structure using content pages.

```
├─ content/
|  └ _global/ # All global fragments are located in this directory
|  └ _index/ # Landing page is in this directory and it's url is changed to **/**.
|  └ about/ # About page
├ layouts/ # You can add extra layout files here. A sample custom fragment is available as a sample.
├ static/ # Your static files are in this directory.
├ themes/ # Hugo uses this directory as a default to look for themes. Syna theme is a git submodule available in this directory.
├ .gitignore
├ .gitmodules
├ config.toml # Hugo config file containing general settings and menu configs.
```

For storing images in the static directory, note that Syna fragments look for
images in their own fragment directory, page directory and `static/images`
directory. Read [resource
fallthrough](https://github.com/okkur/syna/tree/v0.14/docs#image-resource-fallthrough)
docs for more info.

Please read [Syna's
documentation](https://github.com/okkur/syna/tree/v0.14/docs) (Some parts of
documentation may be inaccurate. Let us know if you find any issues.) to
understand how to add fragments and change page data.
