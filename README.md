# sar\_game\_command\_sender

SAR game command sender is a ROS package that allows you to enter game
commands to send to a specific SAR game.

## Usage

`python sar_game_command_sender.py [-h] `

Sends a message to a SAR game. Must have roscore running for the message to be sent.

Optional arguments:

- -h, --help
    - show this help message and exit

## Details about arguments

For more information about these messages, see
[sar\_game\_command\_msgs](https://github.com/sociallyassistiverobotics/sar_game_command_msgs).

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
