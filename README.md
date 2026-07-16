# td27-samples

TeamVapor's drum sample packs, recorded from Eli's Roland TD-27 e-kit
(USB direct, dry, no room ambience). For use with [Strudel](https://strudel.cc/):

```js
samples('github:TeamVapor/td27-samples')

// then the standard drum names play through the real kit:
sound("bd*4, [~ sd]*2, hh*8")
```

## Kits

### punk-rock

One folder per drum, hits ordered **soft → hard**, so the `:n` index is a
velocity dial: `sd:0` is a whisper, `sd:6` is a wallop.

```js
sound("sd:1 sd:6")          // ghost note, then backbeat
n("<2 6>").s("sd")          // same thing, patterned
sound("sd_rim:7")           // marching-band rimshot crack
```

| name | what | samples |
|---|---|---|
| `bd` | kick | 8 |
| `sd` | snare, center | 7 |
| `sd_rim` | snare rimshot | 8 |
| `hh` | hi-hat closed | 7 |
| `oh` | hi-hat open | 6 |
| `ht` `mt` `lt` | high / mid / floor tom | 7 / 7 / 6 |
| `cr` | crash | 5 |
| `rd` | ride | 5 |

Recording/slicing pipeline: see `notes/td27-sampling.md` in
[music-as-code](https://github.com/TeamVapor/music-as-code).

## License note

Personal recordings of a TD-27's preset kit, shared for TeamVapor jam use.
Not a commercial sample product — don't repackage or sell.
