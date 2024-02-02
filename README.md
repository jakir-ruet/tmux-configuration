[![LinkedIn][linkedin-shield-lapissoft]][linkedin-url-lapissoft]
[![Facebook-Page][facebook-shield-lapissoft]][facebook-url-lapissoft]
[![Youtube][youtube-shield-lapissoft]][youtube-url-lapissoft]

## Visit Us [Lapis Soft](http://www.lapissoft.com)

### Terminal Multiplexer (tmux)

tmux is an open-source terminal multiplexer for Unix-like operating systems. It allows multiple terminal sessions to be accessed simultaneously in a single window. It is useful for running more than one command-line program at the same time. It can also be used to detach processes from their controlling terminals, allowing remote sessions to remain active without being visible.

### Install
#### Ubuntu Linux
```bash
sudo apt-get update
sudo apt-get install tmux
```
#### MacOS
```bash
brew update
brew install tmux
```
##### Tmux Plugin Manager Install

https://github.com/tmux-plugins/tpm

#### Version Check
```bash
tmux -V
```
#### Terminal use as tmux
```bash
tmux
```
#### Check location
```bash
command -v tmux
```
### Lets Get Started (t target, a > attach, i > index no )
  |  SL   | Command                                                                                    | Explanation                                             |
  | :---: | :----------------------------------------------------------------------------------------- | :------------------------------------------------------ |
  |   1   | `tmux \ tmux new \ tmux new-session`                                                       | start new as tmux                                       |
  |   2   | `tmux a or tmux at or tmux attach or  tmux attach-session`                                 | attach to last sessions                                 |
  |   3   | `tmux a -t session_name`                                                                   | creates a new tmux session by session-name              |
  |   4   | `tmux ls or tmux list-sessions`                                                            | list of sessions                                        |
  |   5   | `tmux new -s session-name`                                                                 | new session by session name                             |
  |   6   | `tmux kill-ses -t session-name or tmux kill-session -t session-name`                       | kill/delete by session name                             |
  |   7   | `tmux a -t session-name or tmux at -t session-name or tmux attach-session -t session-name` | attach to a session by session-name                     |
  |   5   | `tmux kill-session i`                                                                      | kill a indexed session                                  |
  |   7   | `tmux kill-session -a`                                                                     | kill/delete current session by session-name             |
  |   7   | `tmux kill-session -a -t session-name`                                                     | kill/delete all sessions by session-name                |
  |   7   | `control + b w`                                                                            | session and window preview                              |
  |   7   | `control + b (`                                                                            | move to previous session                                |
  |   7   | `control + b )`                                                                            | move to next session                                    |
  |   2   | `tmux attach -t session_name`                                                              | creates a new tmux session named session_name           |
  |   3   | `tmux switch -t session_name`                                                              | attaches to an existing tmux session named session_name |
  |   6   | `tmux detach (ctl + D)`                                                                    | detach the currently attached session (MacOS)           |
  |   7   | `tmux a -t 0`                                                                              | a for attach, t for target, 0 for zero pane index       |

### tmux consist three sections
- Session: 
  It is collection of windows (terminal). each session has a active window. Sessions are useful for completely separating work environments.

- Window: 
  It is container of panes. tmux has a tabbed interface, but it calls its tabs “Windows”.
  |  SL   | Command                                     | Explanation                       |
  | :---: | :------------------------------------------ | :-------------------------------- |
  |   1   | `tmux new-window (prefix + c)`              | create a new window               |
  |   2   | `tmux select-window -t :0-9 (prefix + 0-9)` | move to the window based on index |
  |   3   | `tmux rename-window (prefix + ,)`           | rename the current window         |

- Pane:
  Panes take my development time from bland to awesome.
  |  SL   | Command                                    | Explanation                                        |
  | :---: | :----------------------------------------- | :------------------------------------------------- |
  |   1   | `tmux split-window (prefix + ")`           | splits the window into two vertical panes          |
  |   2   | `tmux split-window -h (prefix + %)`        | splits the window into two horizontal panes        |
  |   3   | `tmux swap-pane -[UDLR] (prefix + { or })` | swaps pane with another in the specified direction |
  |   4   | `tmux select-pane -[UDLR]`                 | selects the next pane in the specified direction   |
  |   5   | `tmux select-pane -t :.+`                  | selects the next pane in numerical order           |

#### Architecture Terminal Multiplexer (tmux)
![Architecture Terminal Multiplexer (tmux)](/img/tmux-server.png)

#### Other Essential tmux Commands
|  SL   | Command              | Explanation                                            |
| :---: | :------------------- | :----------------------------------------------------- |
|   1   | `tmux list-keys`     | lists out every bound key and the tmux command it runs |
|   2   | `tmux list-commands` | lists out every tmux command and its arguments         |
|   3   | `tmux info`          | lists out every session, window, pane, its pid, etc.   |

#### Exit from a window
```bash
exit
```

### Courtesy of Jakir
[![LinkedIn][linkedin-shield-jakir]][linkedin-url-jakir]
[![Facebook-Page][facebook-shield-jakir]][facebook-url-jakir]
[![Youtube][youtube-shield-jakir]][youtube-url-jakir]

### Have a good day, stay with me
<!-- Personal profile -->

[linkedin-shield-jakir]: https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white
[linkedin-url-jakir]: https://www.linkedin.com/in/jakir-ruet/
[facebook-shield-jakir]: https://img.shields.io/badge/Facebook-%231877F2.svg?style=for-the-badge&logo=Facebook&logoColor=white
[facebook-url-jakir]: https://www.facebook.com/jakir-ruet/
[youtube-shield-jakir]: https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white
[youtube-url-jakir]: https://www.youtube.com/@mjakaria-ruet/featured

<!-- Company profile -->

[linkedin-shield-lapissoft]: https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white
[linkedin-url-lapissoft]: https://www.linkedin.com/company/lapis-soft/
[facebook-shield-lapissoft]: https://img.shields.io/badge/Facebook-%231877F2.svg?style=for-the-badge&logo=Facebook&logoColor=white
[facebook-url-lapissoft]: https://www.facebook.com/GoLapisSoft/
[youtube-shield-lapissoft]: https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white
[youtube-url-lapissoft]: https://www.youtube.com/@LapisSoft/featured
