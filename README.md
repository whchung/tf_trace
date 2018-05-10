# TensorFlow source code trace

- 00: what happens when a TF session is created : TF graph is constructed
- 01: what happens when tf.Session.run() is invoked : XLA ops are registered
- 02: what happens inside DirectSession::Run() : XLA optimization passes are executed
- 03: what happens in XLA optimization passes : XLA clusters are formed
- 04: how XLA graph is lowered to HLO module
- 05: how HLO module is lowered into LLVM IR thru Services
- 06: how LLVM IR are lowered to code objects
- 07: how code objects are loaded and executed
