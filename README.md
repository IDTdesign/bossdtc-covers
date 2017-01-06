# bossdtc-covers

bossrevolution.com hero covers and sliders

## Image naming

In source files (.ai, .psd, .sketch) rename layers to match production filenames on export.
Correct naming important for automation.

Template for naming files:

```
hero_US-ENG_br-club_sm.png
```

where:

* `hero` — prefix, required for automation,
* `US-ENG` is "Culture-Language": `US-SPA`, `UK-ENG`, `DE-GER` etc,
* `br-club` — banner name. Any unique short name. No underscores inside this part,
* `sm` or `md` or `lg` or `thumb` — suffixes for pointing version by size.

All part divided by underscore.

## Image sizes

[Image sizes Giude](http://take.ms/CoAom)

## Algorithm

1. Prepare source files for export.

2. Export images into `src` folder in png 24bit (maximum quality). You will have files:  

    ```
    hero_US-ENG_br-club_lg.png
    hero_US-ENG_br-club_sm.png
    ```

3. Duplicate and rename `hero_US-ENG_br-club_lg.png` → `hero_US-ENG_br-club_md.png`.

4. Open all new `*_md.png` files in Photoshop, crop to 1140×570px and save. Now you have:  

    ```
    hero_US-ENG_br-club_lg.png
    hero_US-ENG_br-club_md.png
    hero_US-ENG_br-club_sm.png
    ```

5. Duplicate and rename `hero_US-ENG_br-club_md.png` → `hero_US-ENG_br-club_thumb.png`.

6. Open all new `*_thumb.png` files in Photoshop, resize to 256×128px and save. Now you have complete set of files:  

    ```
    hero_US-ENG_br-club_lg.png
    hero_US-ENG_br-club_md.png
    hero_US-ENG_br-club_sm.png
    hero_US-ENG_br-club_thumb.png
    ```

7. Copy this set of files to `dist` folder.

8. Compress: convert from png24 to png8 or jpg to reduce file size as much as possible.
