add_llvm_library(LLVMSelectionDAG
  DAGCombiner.cpp
  FastISel.cpp
  FunctionLoweringInfo.cpp
  InstrEmitter.cpp
  LegalizeDAG.cpp
  LegalizeFloatTypes.cpp
  LegalizeIntegerTypes.cpp
  LegalizeTypes.cpp
  LegalizeTypesGeneric.cpp
  LegalizeVectorOps.cpp
  LegalizeVectorTypes.cpp
  ScheduleDAGFast.cpp
  ScheduleDAGList.cpp
  ScheduleDAGRRList.cpp
  ScheduleDAGSDNodes.cpp
  SelectionDAG.cpp
  SelectionDAGBuilder.cpp
  SelectionDAGISel.cpp
  SelectionDAGPrinter.cpp
  TargetLowering.cpp
  TargetSelectionDAGInfo.cpp
  )

add_llvm_library_dependencies(LLVMSelectionDAG
  LLVMAnalysis
  LLVMCodeGen
  LLVMCore
  LLVMMC
  LLVMSupport
  LLVMTarget
  LLVMTransformUtils
  )
