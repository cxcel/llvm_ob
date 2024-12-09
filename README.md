# llvm_ob


wget https://heroims.github.io/obfuscator/NewPass/ollvm14.patch
git clone -b release/14.x git@github.com:llvm/llvm-project.git
cd llvm-project
git apply --reject --ignore-whitespace ../ollvm14.patch

cmake -S llvm -B build -G Ninja
cd build
ninja

