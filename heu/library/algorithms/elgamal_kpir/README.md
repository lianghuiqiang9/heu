
# How to build heu

sh build_wheel_entrypoint.sh

bazel build heu/...

bazel test heu/...


# How to run elgamal_kpir

bazel test //heu/library/algorithms/elgamal_kpir:kpir_test --test_output=all

bazel build //heu/library/algorithms/elgamal_kpir:kpir_test --test_output=all

./bazel-bin/heu/library/algorithms/elgamal_kpir/kpir_test


bazel test //heu/library/algorithms/elgamal_kpir:elgamal_test --test_output=all

bazel build //heu/library/algorithms/elgamal_kpir:elgamal_test --test_output=all

./bazel-bin/heu/library/algorithms/elgamal_kpir/elgamal_test