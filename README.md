# sar\_game\_command\_sender

SAR game command sender is a ROS package that allows you to enter game
commands to send to a specific SAR game.

## Usage

`python sar_game_command_sender.py [-h] [-g {storytelling,s} [{storytelling,s}
...]] [-l LEVEL] {start,s,continue,c,pause,p,end,e,wait,w,skip,k}`

Sends a message to a SAR game. Must have roscore running for the message to be
sent.

Positional arguments:
    - command: {start,s,continue,c,pause,p,end,e,wait,w,skip,k}
        - Specify the command to send.

Optional arguments:

- -h, --help
    - show this help message and exit
- -g {storytelling,s} [{storytelling,s} ...], --game {storytelling,s}
  [{storytelling,s} ...]
    - Which game to send the message to.
- -l LEVEL, --level LEVEL
    - The level the game should start at.

## Details about arguments

For more information about GameCommand messages, see
[sar\_game\_command\_msgs](https://github.com/sociallyassistiverobotics/sar_game_command_msgs).

### Command

Every GameCommand sent needs to include what command to send. The list here is
based on the list of available commands in the `GameCommand` message.

### Game

Every GameCommand should be addressed to a particular SAR game. So far, the
`GameCommand` message definition only lists one game type.

### Level

When sending a `GameCommand.START` message, the game is expected to start at
the level specified by the `level` field. This value should be an integer.


## Version and dependency notes

This program was built and tested with:

- Python 2.7.6
- ROS Indigo
- sar\_game\_command\_msgs (no version number)
- Ubuntu 14.04 LTS (64-bit)

## Bugs and issues

Please report all bugs and issues on the [sar\_game\_command\_sender github
issues
page](https://github.com/personal-robots/sar_game_command_sender/issues).
