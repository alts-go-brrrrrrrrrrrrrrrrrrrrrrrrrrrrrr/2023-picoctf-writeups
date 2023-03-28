# Chrono

## Challenge description:
How to automate tasks to run at intervals on linux servers?

Additional details will be available after launching your challenge instance.

## Solution
The program that the challenge description mentions is `cron`, which allows you to schedule changes at intervals.<br>
Trying `crontab -l` once logged onto the server shows nothing, so I decided to try going to the `/` directory and running `rgrep pico 2>/dev/null` to find the flag.
That does work, and it show that the flag is in /etc/crontab

## Flag
`picoCTF{Sch3DUL7NG_T45K3_L1NUX_7754e199}`
