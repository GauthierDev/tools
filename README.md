---
Google depot tools
---

Source extracted from [depot_tool.git](https://chromium.googlesource.com/chromium/tools/depot_tools.git) to compile plv8
extension and to meet plv8 makefile prerequisites: [plv8 makefile](https://github.com/plv8/plv8/blob/r3.1alpha/Makefile).
In make file google address shhould be modify by decompression path depot_tools.zip : 

```bash
# Get and build the plugin
	cd $(BUILDDIR) \
	&& export PATH=$$PATH:`pwd`/clang+llvm-7.0.1-aarch64-linux-gnu/bin \
	&& wget -nc https://chromium.googlesource.com/chromium/src/+archive/lkgr/tools/clang/plugins.tar.gz \

```
position the caret at any line or the code chunk, then click "+".

The code chunk appears:
```{r}
```

Type any R code in the chunk, for example:
```{r}
mycars <- within(mtcars, { cyl <- ordered(cyl) })
mycars
```

Now, click the **Run** button on the chunk toolbar to [execute](https://www.jetbrains.com/help/pycharm/r-markdown.html#run-r-code) the chunk code. The result should be placed under the chunk.
Click the **Knit and Open Document** to build and preview an output.