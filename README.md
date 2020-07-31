# Wyrd

*Because you're tired of waiting for your bloated calendar program to start up.*

Wyrd is a text-based front-end to Remind, a sophisticated calendar and alarm program available from Roaring Penguin Software, Inc.

Wyrd serves two purposes:
- It displays reminders in a scrollable timetable view suitable for visualizing your calendar at a glance.
- It makes creating and editing reminders fast and easy. However, Wyrd does not hide Remind's textfile programmability, for this is what makes Remind a truly powerful calendaring system.

Wyrd also requires only a fraction of the resources of most calendar programs available today.

## Installation

This section describes how to install Wyrd by compiling from source. Wyrd has been packaged for a number of popular Linux/Unix variants, so you may be able to save yourself some time by installing from a package provided by your OS distribution.

Wyrd is designed to be portable to most Unix-like operating systems, including GNU/Linux, *BSD, and Mac OS X. Before installing Wyrd, your system must have the following software installed:
- OCaml 2 ≥ 3.08
- the ncurses library 3 (and development headers)
- Remind 4 ≥ 3.1.0
- GNU make 5
- the Unix pager application, less

Wyrd may be compiled by executing the following at the root of the source tree:
```bash
./configure
make
```
After compiling, become root and execute
```bash
make install
```
to complete the installation process. The make command here should correspond to GNU make; on some systems (particularly *BSD), you may need to use gmake.
If your ncurses library was built with wide character support, Wyrd can be configured to render UTF-8 encoded reminders. To enable this option, use the command
```bash
./configure --enable-utf8
```
when configuring the sources.

## Notes

2020 note: I fixed compile issues of wyrd in a modern (arch)linux environment, based on haguenau's repository. I am not planning to expand this software, but I'll maintain the AUR package.

Forked from https://github.com/haguenau/wyrd

Original Bazaar repository: https://bazaar.launchpad.net/~pelzlpj/wyrd/wyrd-dev/files


