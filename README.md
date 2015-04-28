# Electricomics `.elcx` File Format

This document serves as a living standard for the Electricomics `.elcx` file format, and is currently in an alpha state.

### Overview

The .elcx file is a container, similar to an iOS app or a Matroska video file.

### Objectives

TBD.

### Inside a container

Inside, the container is structured like this:

```
/images - image assets
/js - supporting javascript libraries
/css - supporting styles
index.html - the file the reader loads when a comic is loaded
comic.json - related metadata and config
```

### Image assets

Images are cropped to 2x retina resolution (4096 x 3072), and supplied in a ​uncompressed ​PSD file to the flatter.
The PSD must consist of two layers, a raw image layer and a vector lettering layer.
When flattened, each distinct "page" should be a 32-bit PNG file with alpha channel enabled. [@TODO: at what DPI/PPI?]

### Authors

- Adam Yeats <adam@ocastastudios.com>

