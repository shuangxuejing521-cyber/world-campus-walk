# campuses/

One folder per campus, named with a short lowercase id (letters, digits, hyphens).

```
campuses/
  hufs/
    campus.json     required: names, location, status, authors
    model.glb       added once a team submits a model under a CC licence
                    (display-only models are hosted outside this repository)
```

## campus.json

| Field | Meaning |
|---|---|
| `id` | Folder name |
| `name` | Campus name in `zh`, `ko`, `en` (add the local language too) |
| `city` | City in `zh`, `ko`, `en` |
| `lat`, `lon` | Latitude and longitude of the model origin |
| `status` | `listed` (marker only), `claimed`, `demo`, `white-box`, `detailed` |
| `team` | Team name, or `null` |
| `authors` | Names credited on the campus page |
| `sources` | Where the geometry came from |
| `licence` | `display-only` (default), `CC-BY-NC-4.0` or `CC-BY-4.0`. See RIGHTS.md |

See `hufs/campus.json` for an example and CONTRIBUTING.md for the model specification.
