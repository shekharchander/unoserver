1.2 (unreleased)
----------------

- Nothing changed yet.


1.1 (2021-10-14)
----------------

- Fixed a bug: If you specified an unknown file extension while piping the
  result to stdout, you would get a type error instead of the correct error.

- Added an extra check that libreoffice is quite dead when exiting,
  I experienced a few cases where soffice.bin was using 100% load in the
  background after unoserver exited. I hope this takes care of that.

- Added ``if __name__ == "main":`` blocks so you can run the modules
  as scripts, and also with ``python3 -m unoserver.server`` and
  ``python3 -m unoserver.converter``.


1.0.1 (2021-09-20)
------------------

- Fixed a bug that meant `unoserver` did not behave well with Supervisord's restart command.


1.0 (2021-08-10)
----------------

- A few small spelling and grammar changes.


1.0b3 (2021-07-01)
------------------

- Make sure `interface` and `port` options are honored.

- Added an --executable option to the server to pick a specific libreoffice installation.

- Changed the infile and outfile options to be positional.

- Added support for using stdin and stdout.

- Added a --convert-to argument to specify the resulting filetype.


1.0b2 (2021-06-24)
------------------

- A bug prevented converting to or from files in the local directory.


1.0b1 (2021-06-24)
------------------

- First beta release


0.0.1 (2021-06-16)
------------------

- First alpha release
