# Color Boxes

A dark Redmine theme built from five bold color boxes: deep shadow purple
backgrounds, electric plum structure, cyan links, glowing amber
call-to-actions and acid green success states.

## Installation

1. Clone this theme ([https://github.com/zaburt/redmine_color_boxes](https://github.com/zaburt/redmine_color_boxes)) into the Redmine `themes/`
   directory at the application root (Redmine 7+) as `color_boxes`:

   ```
   git clone https://github.com/zaburt/redmine_color_boxes.git themes/color_boxes
   ```

   The result should contain:

   ```
   themes/color_boxes/stylesheets/application.css
   ```

   > Note: Redmine 6 and earlier used `public/themes/` instead of `themes/`.

2. Restart Redmine. In production, precompile assets:

   ```
   RAILS_ENV=production bin/rails assets:precompile
   ```

3. Go to `Administration -> Settings -> Display` and select "Color boxes"
   in the "Theme" drop-down list.

## Customize

1. Change `images/logo.svg` for the header/login logo and
   `favicon/favicon.svg` for the browser tab icon.
2. The palette is defined inline as hex values in
   `stylesheets/application.css`. The five base colors:

   | Role                     | Color     |
   |--------------------------|-----------|
   | Deep shadow purple (bg)  | `#1E1625` |
   | Electric plum            | `#4B1F6E` |
   | Cyan neon (links)        | `#158597` (text uses lighter `#35B7CC`) |
   | Glowing amber (actions)  | `#F37024` |
   | Acid green (success)     | `#84C225` |

   Supporting colors:

   | Role                     | Color     |
   |--------------------------|-----------|
   | Page background          | `#141218` / `#171019` |
   | Content / panel bg       | `#1C1A22` / `#26222E` |
   | Text                     | `#EFE8F3` |
   | Muted text               | `#B5A8C4` |
   | Purple accent            | `#9B4FD0` |
   | Light amber              | `#F59A4A` |
   | Error                    | `#E05252` |

   The header, menus, headings, tabs, table headers and panel edges are solid
   color blocks cycling through the palette; page and panel backgrounds are
   neutral dark. The block colors are defined in the last section of
   `stylesheets/application.css` ("Color Boxes — solid color blocks").
3. In production, re-run `assets:precompile` after editing any theme file.

## License

Licensed under [GNU GPLv2](LICENSE).

Copyright (c) 2026 Onur Küçük (onur [at] delipenguen.net)
