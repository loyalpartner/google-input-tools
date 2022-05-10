google-input-tools
==================

This repo contains various of input tools.

Under "chrome/os", it is open source'd input tools for Chromium OS.
Currently there are following input tools:
 - Chinese input methods, the decoding engines are written in pure Javascript.
   - Simplified Chinese Pinyin input method.
   - Traditional Chinese Zhuyin input method.
   - Traditional Chinese Cangjie input method.
 - M17n keyboards.
 - Korean libhangul-based input methods.
 
Under "client", it is open source'd Chinese Pinyin IME for Windows.

Under "cloud", it is JS-based input tools.
Currently there are only M17n keyboards which don't require a cloud service for suggestion decoding.

## Deps Install

1. closure compiler

```bash
curl https://codeload.github.com/google/closure-compiler/tar.gz/refs/tags/maven-release-v20141215  -o  closure-compiler.tar.gz
tar -xvf closure-compiler.tar.gz
cd closure-compiler-maven-release-v20141215
ant jar
```

2. closure library
```
git clone https://github.com/google/closure-library.git
cd closure-library && git checkout 449b74ec05120dd4eb981f8c85c9e54e96488685
sed -i "s/env python$/&2/" **/*.py
```

