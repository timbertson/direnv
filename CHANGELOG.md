
2.1.0 / 2013-11-10 
==================

 * Added support for the fish shell. See README.md for install instructions.
 * Stop recommending using $0 to detect the shell. Fixes #64.
 * Makes the zsh hook resistant to double-hooking.
 * Makes the bash hook resistant to double-hooking.
 * More precise direnv allow error message. Fixes #72

2.0.1 / 2013-07-27 
==================

 * Fixes shell detection corner case

2.0.0 / 2013-06-16
==================

When upgrading from direnv 1.x make sure to restart your shell. The rest is
relatively backward-compatible.

 * changed the execution model. Everything is in a single static executable
 * most of the logic has been rewritten in Go
 * robust shell escaping (supports UTF-8 in env vars)
 * robust eval/export loop, avoids retrys on every prompt if there is an error
 * stdlib: added the `dotenv [PATH]` command to load .env files
 * command: added `direnv reload` to force-reload your environment

