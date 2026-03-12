# Bing `--filterui` Filters Reference


You might want to apply some of Bing's filters, such as filter by license, image size, etc.
BBID doesn't expose to you nice, human readable variants of those, but allows you to utilize all filters exposed by Bing website.
All you need to do is apply filters you want via Bing website and copy them from URL. They are located after `&qft=` and before `&`.

---

## Image Size
| Filter String | Description |
|---|---|
| `+filterui:imagesize-small` | Small images |
| `+filterui:imagesize-medium` | Medium images |
| `+filterui:imagesize-large` | Large images |
| `+filterui:imagesize-wallpaper` | Wallpaper resolution |
| `+filterui:imagesize-custom_WxH` | Custom size, e.g. `custom_1920x1080` |

---

## Aspect Ratio
| Filter String | Description |
|---|---|
| `+filterui:aspect-square` | Square images |
| `+filterui:aspect-wide` | Widescreen / landscape |
| `+filterui:aspect-tall` | Portrait / tall |
| `+filterui:aspect-panoramic` | Panoramic images |

---

## Color
| Filter String | Description |
|---|---|
| `+filterui:color2-bw` | Black & white |
| `+filterui:color2-color` | Color images only |
| `+filterui:color2-red` | Red dominant |
| `+filterui:color2-orange` | Orange dominant |
| `+filterui:color2-yellow` | Yellow dominant |
| `+filterui:color2-green` | Green dominant |
| `+filterui:color2-teal` | Teal dominant |
| `+filterui:color2-blue` | Blue dominant |
| `+filterui:color2-purple` | Purple dominant |
| `+filterui:color2-pink` | Pink dominant |
| `+filterui:color2-brown` | Brown dominant |
| `+filterui:color2-white` | White dominant |
| `+filterui:color2-gray` | Gray dominant |
| `+filterui:color2-black` | Black dominant |

---

## Image Type
| Filter String | Description |
|---|---|
| `+filterui:photo-photo` | Photographs only |
| `+filterui:photo-clipart` | Clipart |
| `+filterui:photo-linedrawing` | Line drawings |
| `+filterui:photo-animatedgif` | Animated GIFs |
| `+filterui:photo-transparent` | Transparent background (PNG) |

---

## License
| Filter String | Description |
|---|---|
| `+filterui:license-L1` | All Creative Commons |
| `+filterui:license-L2` | CC Attribution |
| `+filterui:license-L3` | CC Attribution-ShareAlike |
| `+filterui:license-L4` | CC Attribution-NonCommercial |
| `+filterui:license-L5` | CC Attribution-NoDerivatives |
| `+filterui:license-L6` | CC Attribution-NonCommercial-ShareAlike |
| `+filterui:license-L7` | Public Domain |

---

## Date / Age
| Filter String | Description |
|---|---|
| `+filterui:age-lt1440` | Past 24 hours (1440 min) |
| `+filterui:age-lt10080` | Past week (10080 min) |
| `+filterui:age-lt43200` | Past month (43200 min) |
| `+filterui:age-lt525960` | Past year (525960 min) |

---

## Combining Filters

Filters can be **chained together** with no separator:

```
bbid sunset --filters +filterui:imagesize-large+filterui:color2-orange+filterui:license-L1
```

```
bbid cats --filters +filterui:aspect-square+filterui:photo-photo+filterui:age-lt10080
```