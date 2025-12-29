# NeatoCal - Arabic Edition

A printable calendar with the full year on a single page, with Arabic localization.

Based on [abetusk/neatocal](https://github.com/abetusk/neatocal), which is based on [Neatnik's Calendar](https://neatnik.net/dispenser/?project=calendar).

**Live demo**: [calendar.accelerate.sa](https://calendar.accelerate.sa)

## Features

- RTL (right-to-left) layout
- Arabic-Indic numerals (١٢٣٤٥٦٧٨٩٠)
- Arabic month names and weekday abbreviations
- Friday-Saturday weekend highlighting (default)
- Syriac/Assyrian month names option (كانون، شباط، آذار...)
- UI overlay for year selection and calendar type

## Screenshots

![default](img/neatocal_default.png)

![aligned](img/neatocal_align.png)

## Parameters

| URL Parameter | Description | Example |
|---|---|---|
| `year` | Change year (default to current year) | [...?year=2030](https://calendar.accelerate.sa?year=2030) |
| `start_month` | Start at month other than January. 0 indexed (`0`=Jan, `1`=Feb, ...).  | [...?start_month=7](https://calendar.accelerate.sa?start_month=7) |
| `n_month` | Change number of months to something other than 12 (default `12`).  | [...?n_month=6](https://calendar.accelerate.sa?n_month=6) |
| `layout` | Changes the layout of the calendar. `default` or `aligned-weekdays`.  | [...?layout=aligned-weekdays](https://calendar.accelerate.sa?layout=aligned-weekdays) |
| `start_day` | Start at day other than Sunday. 0 indexed (`0`=Sun, `1`=Mon, ...). Only valid with `aligned-weekdays` layout  | [...?layout=aligned-weekdays&start_day=1](https://calendar.accelerate.sa?layout=aligned-weekdays&start_day=1) |
| `highlight_color` | Change the weekend highlight color (default `eee`) | [...?highlight_color=fee](https://calendar.accelerate.sa?highlight_color=fee) |
| `weekend_days` | Comma separated weekend days. 0 indexed (`0`=Sun, `5`=Fri, `6`=Sat). Default `5,6` | [...?weekend_days=0,6](https://calendar.accelerate.sa?weekend_days=0,6) |
| `rtl` | Enable RTL layout (`true` or `false`). Default `true` | [...?rtl=false](https://calendar.accelerate.sa?rtl=false) |
| `language` | Change the language for month and day codes. | [...?language=ko-KR](https://calendar.accelerate.sa?language=ko-KR) |
| `weekday_code` | Comma separated list of weekday codes. | [...?weekday_code=S,M,T,W,T,F,S](https://calendar.accelerate.sa?weekday_code=S,M,T,W,T,F,S) |
| `month_code` | Comma separated list of month codes. | [...?month_code=J,F,M,A,M,J,J,A,S,O,N,D](https://calendar.accelerate.sa?month_code=J,F,M,A,M,J,J,A,S,O,N,D) |
| `cell_height` | CSS parameter to alter cell height. | [...?cell_height=1.5em](https://calendar.accelerate.sa?cell_height=1.5em) |
| `data` | Location of JSON data file. | [...?data=example/data.json](https://calendar.accelerate.sa?data=example/data.json) |
| `help` | Show help screen  | [...?help](https://calendar.accelerate.sa?help) |

## Credits

- [Neatnik](https://neatnik.net/) - Original calendar concept
- [abetusk/neatocal](https://github.com/abetusk/neatocal) - JavaScript port

## License

MIT
