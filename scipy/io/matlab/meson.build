streams = py3.extension_module('_streams',
  ['_streams.pyx'],
  dependencies: [py3_dep],
  install: true,
  subdir: 'scipy/io/matlab'
)

mio_utils = py3.extension_module('_mio_utils',
  ['_mio_utils.pyx'],
#  c_args: numpy_nodepr_api, TODO: Uncomment once NumPy API usage is fixed
  include_directories: [incdir_numpy],
  dependencies: [py3_dep],
  install: true,
  subdir: 'scipy/io/matlab'
)

mio5_utils = py3.extension_module('_mio5_utils',
  ['_mio5_utils.pyx'],
#  c_args: numpy_nodepr_api, TODO: Uncomment once NumPy API usage is fixed
  include_directories: [incdir_numpy],
  dependencies: [py3_dep],
  install: true,
  subdir: 'scipy/io/matlab'
)

py3.install_sources([
    '__init__.py',
    '_byteordercodes.py',
    '_mio.py',
    '_mio4.py',
    '_mio5.py',
    '_mio5_params.py',
    '_miobase.py',
    'byteordercodes.py',
    'mio.py',
    'mio4.py',
    'mio5.py',
    'mio5_params.py',
    'mio5_utils.py',
    'mio_utils.py',
    'miobase.py',
    'streams.py'
  ],
  pure: false,
  subdir: 'scipy/io/matlab'
)

subdir('tests')
