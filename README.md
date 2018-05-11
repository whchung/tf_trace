# TensorFlow source code trace

- overview_00: very simplified TensorFlow execution model
- overview_01: very simplified TensorFlow XLA execution model
- 00: what happens when a TF session is created : TF graph is constructed
- 01: what happens when tf.Session.run() is invoked : XLA ops are registered
- 02: what happens inside DirectSession::Run() : XLA optimization passes are executed
- 03: how XLA clusters from are formed from a TF graph
- 04: how UserComputation is created from XLA clusters
- 05: how HLO module is created from UserComputation
- 06: how HLO module is optimized
- 07: how HLO module is lowered into LLVM IR
- 08: how LLVM IR is lowered to HSA code object
