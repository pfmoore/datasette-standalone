# A standalone Windows installation of Datasette

See the [project documentation](https://docs.datasette.io/en/stable/)
to get an idea what datasette is. This project provides a standalone
build of datsette that can be run on Windows.

It also allows installing datasette using the [Scoop](https://scoop.sh/)
package manager for Windows.


## Usage

### Manual usage

Download the relevant zipfile for your architecture from the project
release area. Unpack it into a directory of your choice. You can now
run datasette using the extracted `python.exe` as `python -m datasette`.

### Installation with scoop

```bash
scoop bucket add https://github.com/pfmoore/datasette-standalone
scoop install datasette

# Now run datasette
datasette
```

## Release

Documentation for future self.

Update `DATASETTE_VERSION` or `MANIFEST_BUILD_NUMBER` in `main.py`.

(Optional: Update `PYTHON_EMBED_VERSION`.)

Run `py main.py` to generate zip files.

[Create a release](https://github.com/pfmoore/datasette-standalone/releases/new)
and upload the generated zip files.

Update version and URL in `bucket/*.json`.

Push to master.
