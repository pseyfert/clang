set(LLVM_LINK_COMPONENTS
  Support
  )

add_clang_unittest(SemaTests
  ExternalSemaSourceTest.cpp
  )

target_link_libraries(SemaTests
  clangAST
  clangBasic
  clangFrontend
  clangParse
  clangSema
  clangTooling
  )
