1.Custom\_git\_build.sh
-----------------------

Usage:

```bash
$ ./custom_git_build.sh path/to/git/scm/sources
```

2.Unused simple vim plugins managers
------------------------------------

### manage\_vim\_plugins.pl

Stupid vim plugins manager.

Usage:

```bash
perl manage_vim_plugins.pl [OPTIONS]
```

Options:

```bash
--bundle_path=PATH  vim bundles path (default: '~/.vim/bundle')
--plugins=FILENAME  path to the json-file with required plugins (default: 'plugins.json')
--update            update plugin if already exist
-? | --help         show this help, then exit
```

Perl-modules required:

- `JSON::Parse`
- `Getopt::Long`
- `IPC::Cmd`
- `File::Spec`
- `File::HomeDir`
- `File::chdir`
- `File::Path`
- `English`

### update\_vim\_plugins.sh

Dumb vim plugins updater.

Usage:

Just edit plugins.list using template <name>|<url>|<enabled:0|1> and run

```bash
./update_vim_plugins.sh
```

Default bundle path is ~/.vim/bundle.
