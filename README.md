# BiocOpenCRAVAT

Annotation of DNA variants is a crucial and dynamic field in
human disease genetics.  The [OpenCRAVAT system](https://github.com/KarchinLab/open-cravat/wiki)
organizes over 170 'annotators' that resolve queries on features of
genetic variants.

The BiocOpenCRAVAT workspace/workshop materials define interfaces between
Bioconductor data structures and functions and the OpenCRAVAT system, to
simplify the use of OpenCRAVAT annotation by Bioconductor users, and
to simplify aspects of adding new annotation resources to OpenCRAVAT.

- Hit the [Get started](https://vjcitn.github.io/BiocOpenCRAVAT/articles/BiocOpenCRAVAT.html) button to see an interactive catalog of available annotators and converters ...
- See the Articles button for additional documents on the OpenCRAVAT/Bioconductor interface

The oc2bioc R package interfaces the open-cravat Python stack to R.  You can
use this package by pulling the vjcitn/biocopencravat docker container and running
it via

```
docker run -ti vjcitn/biocopencravat bash
```

Start R and then do `library(oc2bioc)`.  Only one open-cravat python module is currently
exposed, `cravat.admin_util$search_remote`, which is called with argument `(".*")` in
`populate_module_set`.  Further work will expose more functionality.

