# Compilers Optimization Bugs reported by BoBpiler Team


| Compiler | Architecture | Bug Type | Link |
| -------- | ------------ | -------- | ---- |
| MSVC | x86-64 | 크래시 | https://developercommunity.visualstudio.com/t/Internal-Compiler-Error-with-for-loop-an/10486573 |
| MSVC | x86-64 | 크래시 | https://developercommunity.visualstudio.com/t/fatal-error-C1001:-Internal-Compiler-Err/10485991?sort=newest |
| MSVC | x86-64 | 부정확한 연산 | https://developercommunity.visualstudio.com/t/O2-and-Ox-Optimizations-Result-in-Incorr/10476654?sort=newest |
| MSVC | x86-64 | 부정확한 연산 | https://developercommunity.visualstudio.com/t/Comparison-of-incorrect-register-values/10480763?sort=newest |
| MSVC | x86-64 | 다른 변수 주소 동일 인식 | https://developercommunity.visualstudio.com/t/Memory-reference-error-due-to-excessive/10477735?sort=newest&page=1 |
| MSVC | x86-64 | 무한 루프 | https://developercommunity.visualstudio.com/t/Optimization-Levels-O1-O2-Ox-Incorrect/10478781?sort=newest |
| MSVC | x86-64 | 부정확한 연산| https://developercommunity.visualstudio.com/t/Incorrectly-compiled-comparison-and-cons/10480723?sort=newest |
| MSVC | x86-64 | 부호 확장 문제 | https://developercommunity.visualstudio.com/t/Incorrect-unsigned-extension-when-upcast/10481317?sort=newest |
| MSVC | x86-64 | 부호 확장 문제 | https://developercommunity.visualstudio.com/t/Impact-of-printf-on-CL-Compiler-Optimiza/10481033?sort=newest |
| MSVC | x86-64 | 지역 변수의 스택 초기화 누락 | https://developercommunity.visualstudio.com/t/Function-pointer-address-comparison-erro/10485960?sort=newest |
| llvm | riscv | 부호 확장 문제 | https://github.com/llvm/llvm-project/issues/68855 |
| llvm | arm64 | 포인터 역참조 생략 | https://github.com/llvm/llvm-project/issues/69294 |
| llvm | mips64el | 부정확한 연산 | https://github.com/llvm/llvm-project/issues/69328 |
| llvm | mips64 | 부정확한 연산 | https://github.com/llvm/llvm-project/issues/70495 |
| gcc | s390x | 부정확한 연산 | https://gcc.gnu.org/bugzilla/show_bug.cgi?id=112112 |
| gcc | s390x | 부정확한 연산 | https://gcc.gnu.org/bugzilla/show_bug.cgi?id=112274 |