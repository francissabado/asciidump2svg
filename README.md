# ASCII Dump (or GDS) to SVG

This project is a branch of the Matthew Beckler's [project](http://www.mbeckler.org/cadence_plot/). The tool can be used with Cadence Virtuoso 5.1 by exporting an ascii dump file as it demonstrates or by generating the asciidump with from a any gds file (e.g exported by Virtuoso 6.1) generated by [gds2ascii](https://github.com/leoheck/gds2ascii). The script requires a configuration file to map layers. The default option is the FreeDPK 45 nm but it can be extended to any design kit.

Required tools
- python
- inkscape

Execution
```bash
asciidump2svg GDS_FILE
```


Main usage example:
```bash
source setup-env.sh
asciidump2svg samples/INV_X1.gds
```

Extra example using [gds2ascii](https://github.com/leoheck/gds2ascii):
```bash
source setup-env.sh
gds2svg samples/INV_X1.gds
```

The output should be an .svg file like this:

<img src="https://cdn.rawgit.com/leoheck/asciidump2svg/master/samples/INV_X1.svg" alt="INV_X1" style="width: 400px;"/>
