add_mlir_dialect_library(TritonNvidiaGPUIR
  Dialect.cpp
  Ops.cpp
  Traits.cpp
  Types.cpp

  DEPENDS
  NVGPUTableGen
  NVGPUAttrDefsIncGen
  TritonNvidiaGPUTableGen
  TritonNvidiaGPUAttrDefsIncGen

  LINK_LIBS PUBLIC
  TritonIR
  TritonGPUIR
)
