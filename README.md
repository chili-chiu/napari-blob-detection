# napari-blob-detection

[![License](https://img.shields.io/pypi/l/napari-blob-detection.svg?color=green)](https://github.com/andy-sweet/napari-blob-detection/raw/main/LICENSE)
[![PyPI](https://img.shields.io/pypi/v/napari-blob-detection.svg?color=green)](https://pypi.org/project/napari-blob-detection)
[![Python Version](https://img.shields.io/pypi/pyversions/napari-blob-detection.svg?color=green)](https://python.org)
[![tests](https://github.com/andy-sweet/napari-blob-detection/workflows/tests/badge.svg)](https://github.com/andy-sweet/napari-blob-detection/actions)
[![codecov](https://codecov.io/gh/andy-sweet/napari-blob-detection/branch/main/graph/badge.svg)](https://codecov.io/gh/andy-sweet/napari-blob-detection)
[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-blob-detection)](https://napari-hub.org/plugins/napari-blob-detection)

Detects blobs in images

----------------------------------

This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.

<!--
Don't miss the full getting started guide to set up your new package:
https://github.com/napari/cookiecutter-napari-plugin#getting-started

and review the napari docs for plugin developers:
https://napari.org/plugins/stable/index.html
-->

This plugin uses [scikit-image's blob detection algorithms](https://scikit-image.org/docs/stable/auto_examples/features_detection/plot_blob.html) to detect bright blobs on dark backgrounds.

Parameters:
image - Image layer for blob detection. Can be a 2D, 3D, or higher dimensionality image.
min_sigma - The smallest blob size to detect
max_sigma - The largest blob size to detect
threshold - The lower the threshold, the more low intensity blobs are detected. 
dimensionality - Users can specify if the image is 2D(+t) or 3D(+t).
algorithm - DOG (Difference of Gaussian)/ LOG (Laplacian of Gaussian)
LOG is the most accurate and slowest approach.
DOG is a faster approximation of LOG approach.

Output:
Blobs are represented by the Points layer. 
The size of each blob is saved under feature['radius']. 

## Installation

You can install `napari-blob-detection` via [pip]:

    pip install napari-blob-detection



To install latest development version :

    pip install git+https://github.com/andy-sweet/napari-blob-detection.git


## Contributing

Contributions are very welcome. Tests can be run with [tox], please ensure
the coverage at least stays the same before you submit a pull request.

## License

Distributed under the terms of the [BSD-3] license,
"napari-blob-detection" is free and open source software

## Issues

If you encounter any problems, please [file an issue] along with a detailed description.

[napari]: https://github.com/napari/napari
[Cookiecutter]: https://github.com/audreyr/cookiecutter
[@napari]: https://github.com/napari
[MIT]: http://opensource.org/licenses/MIT
[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin

[file an issue]: https://github.com/andy-sweet/napari-blob-detection/issues

[napari]: https://github.com/napari/napari
[tox]: https://tox.readthedocs.io/en/latest/
[pip]: https://pypi.org/project/pip/
[PyPI]: https://pypi.org/
