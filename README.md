[![Build Status](https://travis-ci.org/wtanaka/ansible-role-pngnq.svg?branch=master)](https://travis-ci.org/wtanaka/ansible-role-pngcrush)
[![CircleCI](https://circleci.com/gh/wtanaka/ansible-role-pngnq.svg?style=svg)](https://circleci.com/gh/wtanaka/ansible-role-pngcrush)

wtanaka.pngnq
================

This ansible role installs pngnq, an optimizer for PNG (Portable
Network Graphics) files. It can be run from a commandline in an MSDOS
window, or from a UNIX or LINUX commandline.

Its main purpose is to reduce the size of the PNG IDAT datastream by
trying various compression levels and PNG filter methods. It also can
be used to remove unwanted ancillary chunks, or to add certain chunks
including gAMA, tRNS, iCCP, and textual chunks.

Example Playbook
----------------

    - hosts: all
      roles:
         - wtanaka.pngnq

### `pngnq_should_shortcircuit`

Default: True

When `True`, this role short-circuits itself if a `pngnq` is
already in the `PATH`.

### All variables

The full set of configuration options available are visible in
[defaults/main.yml](defaults/main.yml)

License
-------

GPLv2

Author Information
------------------

http://wtanaka.com/
