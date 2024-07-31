---
layout: post
title: Weissman Score
---

# Weissman Score

## In general
How to measure compression? There is score for that.
$$
W = \alpha\frac{r}{\overline r}\frac{\log{\overline T}}{\log{T}}
$$

$ \alpha $ - scaling parameter \
$ r $ - compression ratio $ = \frac{uncompressed\ file\ size}{compressed\ file\ size} $ \
$ T $ - compression time

Overline parameters are same, but for **standard compressor (for reference)**.

Interesing feature is that there is **compression time in equation**. So score depending on it. You can compress much more better with much more time. But there are different needs.

## Features

### Tentative and validated score

**Tentative score** for local debugging, on local data. Testing for PSNR, lossless.

**Validated score** for others to see, on servers using open source data. Testing for all scores.

### Debugging

You can see PSNR for each frame, test for lossless

### Open source

Code is open sourced, datasets are open sourced. **Anyone can prove anyones scores.**

## Tech

Electron with JS for app part. Testing engine in C. It's just for MVP, so that should do.

## MVP

![alt text](weissman.png)

In input section you can specify input data.

`in_path` is path to input file.
`out_path` is path to output file.
`cmd` is command to run your compressor as if you manually type it in terminal to compress `in_path` into `out_path`.

In output section you can see Weissman score and it's parameters.

In debug section you can see log of test. There are will be output from standard compressor and from your compressor so your can debug.

## Personal

Don't even remember how old i am on this photo. Remember that it's me pitching my own compressor on Peer Lab. Spoiler: compressor is trash (i did RLE in every RGB channel, lossless, failed on random data, and not much compression ratio in general). **So to test my compressor i came up with idea of creating Weissman score app.**

Of course i get Weissman score from Silicon Valley series (HBO). Then i don't even think about that there is data compression field. But i am goint crazy about idea of building compressors, it's like you make better oxygen. Every human breathes oxygen, so if you make oxygen better you make everyone better life. Every IT company uses data, and if you make it smaller without loss (or with small loss) you make every company better.

Yeah, i think it's 2016, so i'm 12 years old on this photo. New macbooks are trash and i am with my second hand macbook air 13 2014.

Nice old days, i think then there is my prime. I was doing crazy things, learning everything what is on interenet about programming. 

![alt text](weissman-me.jpeg)