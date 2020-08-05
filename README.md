You might know me for my [writing on zip bombs](https://blog.matthewbarber.io/2019/07/22/how-to-make-compressed-file-quines), which explains compression-algo-tomfoolery with fun and descriptive ASCII charts. Mac users hate me for it [;)](https://twitter.com/_tallison/status/1245100964111159298)

```console
$ hexdump quine.gz > dump.txt
$ cat dump.txt
0000000 1f 8b 08 08 00 00 00 00 00 ff 71 75 69 6e 65 2e
0000020 67 7a 00 00 18 00 e7 ff 1f 8b 08 08 00 00 00 00
0000040 00 ff 71 75 69 6e 65 2e 67 7a 00 00 18 00 e7 ff
0000060 42 16 47 16 07 00 05 00 fa ff 42 16 47 16 07 00
0000100 05 00 fa ff 00 05 00 fa ff 00 14 00 eb ff 42 16
0000120 47 16 07 00 05 00 fa ff 00 05 00 fa ff 00 14 00
0000140 eb ff 42 88 21 c4 00 00 14 00 eb ff 42 88 21 c4
0000160 00 00 14 00 eb ff 42 88 21 c4 00 00 14 00 eb ff
0000200 42 88 21 c4 00 00 14 00 eb ff 42 88 21 c4 00 00
0000220 00 00 ff ff 00 00 00 ff ff 00 0d 00 f2 ff 42 88
0000240 21 c4 00 00 00 00 ff ff 00 00 00 ff ff 00 0d 00
0000260 f2 ff 83 70 a0 1c 00 ff 79 ff a9 cc 00 00 00 83
0000300 70 a0 1c 00 ff 79 ff a9 cc 00 00 00
$ gunzip quine.gz --name
gzip: quine.gz already exists; do you wish to overwrite (y or n)? y
$ hexdump quine.gz > dump2.txt
$ cmp dump.txt dump2.txt ...
omg its a gzip black hole!!
```

I'm currently developing [coinflip](https://github.com/Honno/coinflip), the first randomness testing suite that you'll actually enjoy using.

Looking for a UK graduate job pertaining to software engineering—pop me an [email](mailto:quitesimplymatt@gmail.com) if you're interested!

[matthewbarber.io](https://matthewbarber.io/) 🡸 list of my past software projects
