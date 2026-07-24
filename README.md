# lap-web

The public website for Le LAP, a french nonprofit organization of arcade music
games enthusiasts who decided to rent a location together to put their own
arcade cabinets in.

The location is open to the public about half of the week, times are announced
on Discord.

This website is live at https://lelap.in

More about Le LAP:

- Discord: https://lelap.in/discord
- YouTube: https://www.youtube.com/@LAP_Arcade
- X: https://x.com/LAP_Arcade
- Zenius-i-Vanisher: https://zenius-i-vanisher.com/v5.2/arcade.php?id=8972

## Requirements

- [sssimp](https://pypi.org/project/sssimp/)

Install with your preferred method

```bash
# with pip
pip install sssimp
```

Then run `sssimp`.

If you have `uv` installed, you may want to directly run `uv run sssimp`.

## Scope

This project only handles the static public facing parts, such as the home page
and LAP Contests.

## Documentation

Refer to https://pypi.org/project/sssimp/

**TLDR**, files in `input/content/` get copied to `input/output/`. If they match
certain file extensions, converters are applied to transform them. `.html` files
get treated as Jinja templates. Data in `input/data/` is made available to
templates. Check the README for more information.

## License

MIT.
