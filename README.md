# TensorFlow source code trace

- 00: what happens when a TF session is created : TF graph is constructed
- 01: what happens when tf.Session.run() is invoked : XLA ops are registered
- 02: what happens inside DirectSession::Run() : XLA optimization passes are executed
- 03: how XLA clusters from are formed from a TF graph
- 04: how UserComputation is created from XLA clusters
- 05: how HLO module is created from UserComputation
- 06: how HLO module is lowered into LLVM IR
- 07: how LLVM IR are lowered to code objects
