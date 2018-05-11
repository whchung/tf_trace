# TensorFlow source code trace

Overview:
- [overview_00](svg/overview_00.svg): very simplified TensorFlow execution model
- [overview_01](svg/overview_01.svg): very simplified TensorFlow XLA execution model
- [overview_02](svg/overview_02.svg): very simplified TensorRT execution model

Deep dive:
- [00](svg/00.svg): what happens when a TF session is created : TF graph is constructed
- [01](svg/01.svg): what happens when tf.Session.run() is invoked : XLA device is registered
- [02](svg/02.svg): what happens inside DirectSession::Run() : XLA optimization passes are executed
- [03](svg/03.svg): how XLA clusters from are formed from a TF graph
- [04](svg/04.svg): how UserComputation is created from XLA clusters
- [05](svg/05.svg): how HLO module is created from UserComputation
- [06](svg/06.svg): how HLO module is optimized
- [07](svg/07.svg): how HLO module is lowered into LLVM IR
- [08](svg/08.svg): how LLVM IR is lowered to HSA code object

# Build

```
dot -Tsvg -o svg/foo.svg foo.dot
```
