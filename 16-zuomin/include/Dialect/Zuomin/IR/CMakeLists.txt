set(LLVM_TARGET_DEFINITIONS ZuominDialect.td)
# 生成Zuomin Dialect 的声明
mlir_tablegen(ZuominDialect.h.inc --gen-dialect-decls -dialect=zuomin)
# 生成Zuomin Dialect 的实现
mlir_tablegen(ZuominDialect.cpp.inc --gen-dialect-defs -dialect=zuomin)

# 将生成的命令们定义为为target
add_public_tablegen_target(ZuominDialectIncGen)


