# NAME

Dist::Zilla::Plugin::Test::EOF - Check that all files in the projects end correctly

<div>
    <p>
    <img src="https://img.shields.io/badge/perl-5.10+-blue.svg" alt="Requires Perl 5.10+" />
    <a href="https://travis-ci.org/Csson/p5-dist-zilla-plugin-test-eof"><img src="https://api.travis-ci.org/Csson/p5-dist-zilla-plugin-test-eof.svg?branch=master" alt="Travis status" /></a>
    <a href="http://cpants.cpanauthors.org/release/CSSON/Dist-Zilla-Plugin-Test-EOF-0.0600"><img src="http://badgedepot.code301.com/badge/kwalitee/CSSON/Dist-Zilla-Plugin-Test-EOF/0.0600" alt="Distribution kwalitee" /></a>
    <a href="http://matrix.cpantesters.org/?dist=Dist-Zilla-Plugin-Test-EOF%200.0600"><img src="http://badgedepot.code301.com/badge/cpantesters/Dist-Zilla-Plugin-Test-EOF/0.0600" alt="CPAN Testers result" /></a>
    </p>
</div>

# VERSION

Version 0.0600, released 2018-07-31.

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

This software is copyright (c) 2018 by Erik Carlsson.

This is free software; you can redistribute it and/or modify it under
the same terms as the Perl 5 programming language system itself.
