# money-ware

## Challenge description
Flag format: picoCTF{Malwarename} The first letter of the malware name should be capitalized and the rest lowercase. Your friend just got hacked and has been asked to pay some bitcoins to 1Mz7153HMuxXTuR2R1t78mGSdzaAtNbBWX. He doesn’t seem to understand what is going on and asks you for advice. Can you identify what malware he’s being a victim of?

## Solution
Googling `1Mz7153HMuxXTuR2R1t78mGSdzaAtNbBWX` shows the blockchain explorer for that address, and the Bitcoin abuse database site for that address [here](https://www.bitcoinabuse.com/reports/1Mz7153HMuxXTuR2R1t78mGSdzaAtNbBWX). The bottommost entry is `More information here: https://blog.avira.com/petya-strikes-back/`<br>
The malware name is `petya`

## Flag
`picoCTF{petya}`
