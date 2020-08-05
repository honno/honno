You might know me for my [writing on zip bombs](https://blog.matthewbarber.io/2019/07/22/how-to-make-compressed-file-quines), which explains compression-algo-tomfoolery with fun and descriptive ASCII charts. macOS users hate me for it [<sub>;)</sub>](https://twitter.com/_tallison/status/1245100964111159298)

```console
honno:~$ hexdump quine.gz > dump.txt
honno:~$ head -2 dump.txt; echo "..."; tail -2 dump.txt;
0000000 1f 8b 08 08 00 00 00 00 00 ff 71 75 69 6e 65 2e
0000020 67 7a 00 00 18 00 e7 ff 1f 8b 08 08 00 00 00 00
...
0000260 f2 ff 83 70 a0 1c 00 ff 79 ff a9 cc 00 00 00 83
0000300 70 a0 1c 00 ff 79 ff a9 cc 00 00 00
honno:~$ gunzip quine.gz --name
gzip: quine.gz already exists; do you wish to overwrite (y or n)? y
honno:~$ hexdump quine.gz > dump2.txt
honno:~$ cmp dump.txt dump2.txt ...
zomg its a gzip black hole!!
```

I'm currently developing [**coinflip**](https://github.com/Honno/coinflip), the first randomness testing suite that you'll actually enjoy using.

Looking for a graduate job pertaining to software engineering, UK or abroad—pop me an [email](mailto:quitesimplymatt@gmail.com) if you're interested!
