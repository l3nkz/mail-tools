# Mail-Tools

This repository contains a collection of tools which I use for my local mail setup.

## mcount

This script watches a maildir and counts the number of unread mails. The number itself can be
requested from the script via a D-Bus interface.

## mmanage

This script can be used to clean up folders with a lot of mails. The aim of the script is to
remove mails from a maildir which are older than a particular number of days. These mails can
be either directly removed or archived into a different folder. The script also supports a
dry-run operation. An additional feature of the script is, that it tries to keep threads together.
A mail belonging to a thread is only deleted (or archived) of all mails of this thread are older
than the specified number of days. Accordingly, one never looses track if its mails.

## mnotify

This script watches a maildir and triggers on-screen notifications whenever there is a new mail.
