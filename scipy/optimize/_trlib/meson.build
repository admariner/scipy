_trlib = py3.extension_module('_trlib',
  [
    '_trlib.pyx',
    'trlib_krylov.c',
    'trlib_eigen_inverse.c',
    'trlib_leftmost.c',
    'trlib_quadratic_zero.c',
    'trlib_tri_factor.c'
  ],
  c_args: numpy_nodepr_api,
  dependencies: [py3_dep, lapack],
  include_directories: [
    inc_np,
    '../../_lib',
    '../../_build_utils/src'
  ],
  install: true,
  subdir: 'scipy/optimize/_trlib'
)

py3.install_sources(
  ['__init__.py'],
  pure: false,
  subdir: 'scipy/optimize/_trlib'
)
