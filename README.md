# NAME

Mojolicious::Command::listdeps - Command to list dependencies for a 
Mojolicious project

# VERSION

Version 0.07

# DESCRIPTION

[Mojolicious::Command::listdeps](https://metacpan.org/pod/Mojolicious::Command::listdeps) lists all module dependencies, and
is typically invoked from the command line in the root of your
[Mojolicious](https://metacpan.org/pod/Mojolicious) project

# SYNOPSIS

    use Mojolicious::Command::listdeps;

    my $command = Mojolicious::Command::listdeps->new;
    $command->run(@ARGV);

# COMMANDLINE OPTIONS

The listdeps command supports the following command line options:

- --include-tests

    Include dependencies required for tests

- --missing

    Only list missing modules

- --skip-lib

    Do not list modules found in ./lib as a dependency

- --verbose

    List additional information

- --core

    Include core modules in list

- --cpanfile

    Create or append module information to cpanfile

# ATTRIBUTES

[Mojolicious::Command::listdeps](https://metacpan.org/pod/Mojolicious::Command::listdeps) inherits the following attributes
from [Mojolicious::Command](https://metacpan.org/pod/Mojolicious::Command)

## `description`

Short description displayed in the "mojo" command list

## `usage`

Displayed in response to mojo help listdeps

# METHODS

[Mojolicious::Command::listdeps](https://metacpan.org/pod/Mojolicious::Command::listdeps) inherits its methods from 
from [Mojolicious::Command](https://metacpan.org/pod/Mojolicious::Command)

## `run`

    $command->run;
    $command->run(@ARGV);

Used to invoke the command.

# SEE ALSO

[Mojolicious](https://metacpan.org/pod/Mojolicious), [Mojolicious::Guides](https://metacpan.org/pod/Mojolicious::Guides), [http://mojolicio.us](http://mojolicio.us).

# THANKS

This module was inspired by the listdeps command in [Dist::Zilla](https://metacpan.org/pod/Dist::Zilla) 
