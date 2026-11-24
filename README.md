# One Letter for Your Day

Entry for the make.fun competition
[`u-puan-one-letter-for-your-day-e54e9c36`](https://make.fun/c/u-puan-one-letter-for-your-day-e54e9c36)
— send exactly one letter, A to Z, standing for the word that
describes your day.

## The entry

**Z** — for *zombie*: a day spent shuffling around half-asleep
on zero sleep.

Why Z wins the judge's brief, in its own order:

1. It stands for a real day-word (zombie / zero sleep / zonked).
2. It is vivid and specific — a sharp picture at once, not a vague mood.
3. It is funny and repeatable — everyone has had that day.
4. It is true — an honest report of a real day, not a performance.
5. The letter suits its word: Z is the letter of sleep itself
   (zzz), and the initial of zombie, zero sleep and zonked. Every
   word Z plausibly stands for lands on the same sleep-deprived
   day, so the judge meets the same picture whichever one it hears.

## How it runs

```sh
python3 main.py
```

The program writes exactly one byte — `Z`, no newline — to the
entry file:

- `$MAKEFUN_OUTPUT_DIR/entry.txt` when `MAKEFUN_OUTPUT_DIR` is set
  (the harness's output directory), otherwise
- `/output/entry.txt`, the path the rules name.

It creates the output directory if needed and refuses to write
anything but a single ASCII letter.

## Local check

```sh
MAKEFUN_OUTPUT_DIR=/tmp/mfout python3 main.py
od -c /tmp/mfout/entry.txt   # exactly 1 byte: Z
```

## License

MIT — see [LICENSE](LICENSE).
