# Copyright 2020 the V8 project authors. All rights reserved.
# Use of this source code is governed by a BSD-style license that can be
# found in the LICENSE file.
gclient_gn_args_file = 'v8-gn-example/build/config/gclient_args.gni'

gclient_gn_args = [
  'checkout_google_benchmark',
]

vars = {
  'checkout_google_benchmark' : False,

  'abseil_cpp_revision': '66b870c3b1cbbb7f85b31cc9a8a785329f5ebcb8',
  'abseil_cpp_url': 'https://chromium.googlesource.com/chromium/src/third_party/abseil-cpp.git',

  'build_revision': 'ae5b5ecabdc944bde2730e6b7d13abe71ca9a2ee',
  'build_url': 'https://chromium.googlesource.com/chromium/src/build.git',

  'buildtools_revision': '4be464e050b3d05060471788f926b34c641db9fd',
  'buildtools_url': 'https://chromium.googlesource.com/chromium/src/buildtools.git',

  'buildtools_clang_format_revision': 'bb994c6f067340c1135eb43eed84f4b33cfa7397',
  'buildtools_clang_format_url': 'https://chromium.googlesource.com/chromium/llvm-project/cfe/tools/clang-format.git',

  'buildtools_libcxx_revision': '78d6a7767ed57b50122a161b91f59f19c9bd0d19',
  'buildtools_libcxx_url': 'https://chromium.googlesource.com/chromium/llvm-project/libcxx.git',

  'buildtools_libcxxabi_revision': 'ce3db128f9e4d6d19d1cdbe39bb45fcc64a5adb0',
  'buildtools_libcxxabi_url': 'https://chromium.googlesource.com/chromium/llvm-project/libcxxabi.git',

  'buildtools_libunwind_revision': '3e6ec2ae9afaa3683269b690612f84d907943ea2',
  'buildtools_libunwind_url': 'https://chromium.googlesource.com/external/llvm.org/libunwind.git',

  'clang_revision': 'd4827bfe100154b06d9ffa59b21bb845fce9c7d5',
  'clang_url': 'https://chromium.googlesource.com/chromium/src/tools/clang.git',

  'depot_tools_revision': '6e970e597b25a3a74a560746711d1811133841d2',
  'depot_tools_url': 'https://chromium.googlesource.com/chromium/tools/depot_tools.git',

  # GN CIPD package version.
  'gn_version': 'git_revision:81ee1967d3fcbc829bac1c005c3da59739c88df9',

  'googletest_revision': '07f4869221012b16b7f9ee685d94856e1fc9f361',
  'googletest_url': 'https://chromium.googlesource.com/external/github.com/google/googletest.git',

  'icu_revision': '7db579a73addda0edb2bb83465ae51bcdc601af7',
  'icu_url': 'https://chromium.googlesource.com/chromium/deps/icu.git',

  'jinja2_revision': 'a82a4944a7f2496639f34a89c9923be5908b80aa',
  'jinja2_url': 'https://chromium.googlesource.com/chromium/src/third_party/jinja2.git',

  'markupsafe_revision': 'f2fb0f21ef1e1d4ffd43be8c63fc3d4928dea7ab',
  'markupsafe_url': 'https://chromium.googlesource.com/chromium/src/third_party/markupsafe.git',

  'trace_common_revision' : 'ea3ab7b3f22a844966f27bcafc0475e4ea95a019',
  'trace_common_url': 'https://chromium.googlesource.com/chromium/src/base/trace_event/common.git',

  'v8_revision': 'bc0bfbe84059da4989474e1bbe1282ebcf72886d',
  'v8_url': 'https://chromium.googlesource.com/v8/v8.git',

  'zlib_revision': 'd7f3ca98b2b0d5f72656502961a59353791c4f8a',
  'zlib_url': 'https://chromium.googlesource.com/chromium/src/third_party/zlib.git',
}
deps = {
  'v8-gn-example/base/trace_event/common': Var('trace_common_url') + '@' + Var('trace_common_revision'),
  'v8-gn-example/build': Var('build_url') + '@' + Var('build_revision'),
  'v8-gn-example/buildtools': Var('buildtools_url') + '@' + Var('buildtools_revision'),
  'v8-gn-example/buildtools/clang_format/script': Var('buildtools_clang_format_url') + '@' + Var('buildtools_clang_format_revision'),
  'v8-gn-example/buildtools/third_party/libc++/trunk': Var('buildtools_libcxx_url') + '@' + Var('buildtools_libcxx_revision'),
  'v8-gn-example/buildtools/third_party/libc++abi/trunk': Var('buildtools_libcxxabi_url') + '@' + Var('buildtools_libcxxabi_revision'),
  'v8-gn-example/buildtools/third_party/libunwind/trunk': Var('buildtools_libunwind_url') + '@' + Var('buildtools_libunwind_revision'),
  'v8-gn-example/third_party/abseil-cpp': Var('abseil_cpp_url') + '@' + Var('abseil_cpp_revision'),
  'v8-gn-example/third_party/depot_tools': Var('depot_tools_url') + '@' + Var('depot_tools_revision'),
  'v8-gn-example/third_party/googletest/src': Var('googletest_url') + '@' + Var('googletest_revision'),
  'v8-gn-example/third_party/icu': Var('icu_url') + '@' + Var('icu_revision'),
  'v8-gn-example/third_party/jinja2': Var('jinja2_url') + '@' + Var('jinja2_revision'),
  'v8-gn-example/third_party/markupsafe': Var('markupsafe_url') + '@' + Var('markupsafe_revision'),
  'v8-gn-example/third_party/zlib': Var('zlib_url') + '@' + Var('zlib_revision'),
  'v8-gn-example/tools/clang': Var('clang_url') + '@' + Var('clang_revision'),
  'v8-gn-example/v8': Var('v8_url') + '@' +  Var('v8_revision'),
  'v8-gn-example/buildtools/linux64': {
    'packages': [
      {
        'package': 'gn/gn/linux-amd64',
        'version': Var('gn_version'),
      }
    ],
    'dep_type': 'cipd',
    'condition': 'host_os == "linux"',
  },
  'v8-gn-example/buildtools/mac': {
    'packages': [
      {
        'package': 'gn/gn/mac-amd64',
        'version': Var('gn_version'),
      }
    ],
    'dep_type': 'cipd',
    'condition': 'host_os == "mac"',
  },
  'v8-gn-example/buildtools/win': {
    'packages': [
      {
        'package': 'gn/gn/windows-amd64',
        'version': Var('gn_version'),
      }
    ],
    'dep_type': 'cipd',
    'condition': 'host_os == "win"',
  },
}

hooks = [
  {
    # Update the Windows toolchain if necessary.
    'name': 'win_toolchain',
    'pattern': '.',
    'condition': 'checkout_win',
    'action': ['python', 'v8-gn-example/build/vs_toolchain.py', 'update'],
  },
  {
    # Update the Mac toolchain if necessary.
    'name': 'mac_toolchain',
    'pattern': '.',
    'condition': 'checkout_mac',
    'action': ['python', 'v8-gn-example/build/mac_toolchain.py'],
  },
  {
    'name': 'clang',
    'pattern': '.',
    'action': ['python', 'v8-gn-example/tools/clang/scripts/update.py'],
  },
  {
    # Update LASTCHANGE.
    'name': 'lastchange',
    'pattern': '.',
    'action': ['python', 'v8-gn-example/build/util/lastchange.py',
               '-o', 'v8-gn-example/build/util/LASTCHANGE'],
  },
  {
    'name': 'sysroot_x64',
    'pattern': '.',
    'condition': 'checkout_linux and checkout_x64',
    'action': ['python',
               'v8-gn-example/build/linux/sysroot_scripts/install-sysroot.py',
               '--arch=x64'],
  },
]