# Salt

The purpose of this repository is to maintain Salt Project code to manage my virtual machines.

## Environment setup
I will be attempting to use Salt in a 'masterless' setup, meaning my virtual machines are simple minions who pull state files from this repository periodically and apply the high state.  The intent is to have an idempotent configuration management system in which configuration drift is minimized.

The 'dev' branch will be used to test configuration changes on a local virtual machine.  The 'main' branch will be used for hosts in production (AWS).

## Useful commands
On the minion

- `salt-call --local <salt-command>`

