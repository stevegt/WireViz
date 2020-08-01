# (Re-)Building the example projects

<!--
The following text is taken from #118
https://github.com/formatc1702/WireViz/pull/118

TODO: write a better explaination -->


- Run `python build_examples.py` to build generated files in all groups.
- Run `python build_examples.py compare` to compare generated files in all groups against the last commit.
- Run `python build_examples.py clean` to delete generated files in all groups.
- Run `python build_examples.py restore` to restore generated files in all groups from the last commit.
- Edit 4: Append `-c` or `--compare-graphviz-output` to the `compare` command above to also compare the Graphviz output (default: False).
- Append `-g` or `--groups` followed by space separated group names to any command above, and the set of generated files affected by the command will be limited to the selected groups.
- Run `python build_examples.py -h` or with `--help` to print the generated help. The auto-generated help text is not the best, but better than maintaining it manually. I wonder if [click](https://click.palletsprojects.com/en/7.x/) as recommended in https://github.com/formatc1702/WireViz/issues/60#issuecomment-663278159 could improve this?
