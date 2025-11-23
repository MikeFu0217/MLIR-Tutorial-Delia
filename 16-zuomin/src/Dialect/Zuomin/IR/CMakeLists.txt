add_mlir_dialect_library(MLIRZuominDialect${ch_num}
    ZuominDialect.cpp

    DEPENDS
    ZuominDialectIncGen${ch_num}

    LINK_LIBS PUBLIC
    MLIRIR
    MLIRTensorDialect
)

