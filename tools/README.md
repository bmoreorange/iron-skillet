# Using the tools

To build a full configuration from the supplied configuration snippets:

```bash
cd tools
python3 ./build_full_templates.py
```


The resulting templates are stored in the `full` directory as `iron_skillet_day1_template.xml`


To create loadable template files with variable substitutions:

```
vi my_variables.py   [Edit variables to the local environment]
python3 ./build_my_templates.py
```

The output loadable templates are in the `templates/my_configs` directory with name as `template name` + `datetime`.

Each run results in a new archive directory allowing for new configs with modified variables.
