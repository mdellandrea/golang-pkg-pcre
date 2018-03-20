golang-pkg-pcre
===============

This is a Go language package providing Perl-Compatible RegularExpression
support using libpcre++.  Install the package with the current Debian
distribution as follows:

    sudo apt-get install libpcre++-dev
    go get github.com/glenn-brown/golang-pkg-pcre/src/pkg/pcre

Go programs that depend on this package should import this package as
follows to allow automatic downloading:

    import "github.com/glenn-brown/golang-pkg-pcre/src/pkg/pcre"

This is based off of previous work by Florian Weimer and Glenn Brown. It adds `BReset()` which gives back the boolean result when resetting a Matcher. It also adds convenience methods for retrieving the left index and right index of a match `LIndex()` and `RIndex()` respectively.
