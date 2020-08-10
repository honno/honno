You might know me for my [writing on recursive gzip bombs](https://blog.matthewbarber.io/2019/07/22/how-to-make-compressed-file-quines), where we made ⚠ [quine.gz](https://blog.matthewbarber.io/downloads/quine.gz) ⚠ together. I'm particularly proud of how I teach compression-algorithm-tomfoolery with fun and descriptive ASCII charts. My recursive compressed file is used in testing Apache's [Tika](https://tika.apache.org/) project, and is currently [wreaking havoc](https://twitter.com/_tallison/status/1245100964111159298) on modern Mac systems 😈

```console
honno:~$ hexdump quine.gz > dump.txt
honno:~$ head -2 dump.txt; tail -2 dump.txt;
0000000 1f 8b 08 08 00 00 00 00 00 ff 71 75 69 6e 65 2e
0000020 67 7a 00 00 18 00 e7 ff 1f 8b 08 08 00 00 00 00
0000260 f2 ff 83 70 a0 1c 00 ff 79 ff a9 cc 00 00 00 83
0000300 70 a0 1c 00 ff 79 ff a9 cc 00 00 00
honno:~$ gunzip quine.gz --name
gzip: quine.gz already exists; do you wish to overwrite (y or n)? y
honno:~$ hexdump quine.gz > dump2.txt
honno:~$ cmp dump.txt dump2.txt && echo ":) it matches!!" || echo "did not match :("
:) it matches!!
```

Nowadays I'm developing [**coinflip**](https://github.com/Honno/coinflip), a randomness testing suite made in Python. It started as my undergrad thesis project, with my final report available as [📜 PDF](https://raw.githubusercontent.com/Honno/coinflip/report/report.pdf), and my presentation available on [▶ YouTube](https://www.youtube.com/watch?v=0xrWG3Ki9Z8).

I'm looking for a graduate role, UK or abroad—pop me an [email](mailto:quitesimplymatt@gmail.com) if you're interested in hiring me! My résumé is available [here](https://matthewbarber.io/assets/home/matthew-barber-cv-online.pdf) :)
