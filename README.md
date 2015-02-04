# NAME

Dist::Zilla::Plugin::Test::EOF - Check that all files in the projects end correctly

# VERSION

Version 0.0501, released 2015-02-04.

# SYNOPSIS

    [Test::EOF]
    strict = 1

# DESCRIPTION

Generates author tests using [Test::EOF](https://metacpan.org/pod/Test::EOF). It checks that all Perl files end with the requested amount of new lines. It assumes that all linebreaks only consist of `\n`. It does not check
for any other line break character - use [Dist::Zilla::Plugin::Test::EOL](https://metacpan.org/pod/Dist::Zilla::Plugin::Test::EOL) for that.

## ATTRIBUTES

The following attributes are accepted:

**`minimum_newlines`**

Default: `1`

The lowest amount of newlines acceptable at end-of-file.

**`maximum_newlines`**

Default: `minimum_newlines + 3`

The highest amount of newlines acceptable at end-of-file.

**`strict`**

Default: `0`

If true, sets both `minimum_newlines` and `maximum_newlines` to `1`. This option has precedence.

# SEE ALSO

[Dist::Zilla::Plugin::Test::EOL](https://metacpan.org/pod/Dist::Zilla::Plugin::Test::EOL)

# SOURCE

[https://github.com/Csson/p5-dist-zilla-plugin-test-eof](https://github.com/Csson/p5-dist-zilla-plugin-test-eof)

# HOMEPAGE

[https://metacpan.org/release/Dist-Zilla-Plugin-Test-EOF](https://metacpan.org/release/Dist-Zilla-Plugin-Test-EOF)

# AUTHOR

Erik Carlsson <info@code301.com>

# COPYRIGHT AND LICENSE

This software is copyright (c) 2015 by Erik Carlsson <info@code301.com>.

This is free software; you can redistribute it and/or modify it under
the same terms as the Perl 5 programming language system itself.
