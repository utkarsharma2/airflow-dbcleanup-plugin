# astronomer-airflow-dbcleanup-plugin

An Apache Airflow plugin that exposes an rest endpoint to perform cleanup on airflow tables.

## How do I test this repo

You must have the astro CLI installed.

1. Clone the repo
2. Run `astro dev init`
3. Create a directory and copy some files into the `plugins/` directory of your Astro project:
   ```bash
   mkdir plugins/astronomer_dbcleanup_plugin
   cp *.py plugins/astronomer_dbcleanup_plugin/
   ```
4. Run `astro dev start`

## Publishing new packages to GitHub

1. Update the `__version__` variable in `dbcleanup_plugin.py`
2. Run `python -m build`
3. Upload the generated Wheel (`.whl`) and `.tar.gz` files generated in `dist/` to GitHub as a release
