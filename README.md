# mklink for Windows Bash

Bash script to invoke Windows [`mklink`] command under elevated privileges.

## Requirements

- A Bash interpreter for Windows, such as the one bundled with [Git for
  Windows].

## Usage

- Copy `bash-mklink` to a folder in your terminal `$PATH`, for instance
  `$HOME/bin` if you are using [Git Bash].

- Invoke it as:

      bash-mklink LINK TARGET

  where `LINK` and `TARGET` are Unix paths; the command will internally convert
  them to Windows paths and then prompt you for Administrator authorization.

## TODO

- Support original `mklink` options, at least `/j`.
- Return the command output to the calling shell.
- Allow creating links to relative targets.
- Provide a script to replace `ln`.


[`mklink`]: https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/mklink
[Git for Windows]: https://gitforwindows.org/
[Git Bash]: https://gitforwindows.org/#bash
