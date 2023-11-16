# 컴파일러 최적화 버그 제보
## List of Compiler Optimization Bugs Reported by BoBpiler Team

이 문서는 BoBpiler 팀이 발견하고 보고한 다양한 컴파일러의 최적화 버그들을 모아놓은 목록입니다. 각 컴파일러, 아키텍처, 버그 유형 및 상세 링크를 포함하고 있습니다. 이러한 버그 리포트는 해당 분야의 전문가들이 문제를 해결하고 소프트웨어 개발 과정에서 발생할 수 있는 유사한 문제와 잠재적인 보안 취약점을 예방하는 데 기여할 수 있습니다.

This document contains a compilation of optimization bugs in various compilers discovered and reported by the BoBpiler Team. It includes the compiler, architecture, type of bug, and a link to further details. Each bug report can assist experts in resolving issues, thereby helping to prevent similar issues and potential security vulnerabilities in the software development process.

---
| Compiler | Arch | Bug Type | Link |
| --- | --- | --------------------------- | ---- |
| GCC | s390x |     Inaccurate Computation (부정확한 연산)    | [Details](https://gcc.gnu.org/bugzilla/show_bug.cgi?id=112112) |
| GCC | s390x |     Inaccurate Computation (부정확한 연산)    | [Details](https://gcc.gnu.org/bugzilla/show_bug.cgi?id=112274) |
| GCC | s390x |     Inaccurate Computation (부정확한 연산)    | [Details](https://gcc.gnu.org/bugzilla/show_bug.cgi?id=112329) |
| LLVM | x86-64 |   Infinite Loop Elimination (무한 루프 제거)    | [Details](https://github.com/llvm/llvm-project/issues/66307) |
| LLVM | arm64 |    Pointer Dereference Omission (포인터 역참조 생략)   | [Details](https://github.com/llvm/llvm-project/issues/69294) |
| LLVM | riscv |    Sign/Unsign Extension Issue (부호 확장 문제)   | [Details](https://github.com/llvm/llvm-project/issues/68855) |
| LLVM | powerpc64 |    Sign/Unsign Extension Issue (부호 확장 문제)   | [Details](https://github.com/llvm/llvm-project/issues/71030) |
| LLVM | mips64el |     Inaccurate Computation (부정확한 연산)    | [Details](https://github.com/llvm/llvm-project/issues/69328) |
| LLVM | mips64 |   Inaccurate Computation (부정확한 연산)    | [Details](https://github.com/llvm/llvm-project/issues/70495) |
| LLVM | s390x |    Inaccurate Computation (부정확한 연산)    | [Details](https://github.com/llvm/llvm-project/issues/72018) |
| MSVC | arm64 |    Inaccurate Computation (부정확한 연산)    | [Details](https://developercommunity.visualstudio.com/t/C-ARM64-Optimization-Bug/10503910) |
| MSVC | arm64 |    Inaccurate Computation (부정확한 연산)    | [Details](https://developercommunity.visualstudio.com/t/Inconsistent-Outputs-in-ARM64-C-Progra/10505191) |
| MSVC | arm64 |    Inaccurate Computation (부정확한 연산)    | [Details](https://developercommunity.visualstudio.com/t/ARM64-MSVC-Compiler-Optimization-Leads-t/10508262) |
| MSVC | arm64 |    Inaccurate Computation (부정확한 연산)    | [Details](https://developercommunity.visualstudio.com/t/MSVC-ARM64-Compiler-Incorrectly-Optimize/10510611) |
| MSVC | x86-64 |   Incorrect Inline Call Order (부정확한 인라인 호출 순서)    | [Details](https://developercommunity.visualstudio.com/t/O1-Optimization-Leads-to-Incorrect-Funct/10469220?sort=newest) |
| MSVC | x86-64 |   Misidentification of Different Variable Addresses (다른 변수 주소 동일 인식)     | [Details](https://developercommunity.visualstudio.com/t/Memory-reference-error-due-to-excessive/10477735?sort=newest&page=1) |
| MSVC | x86-64 |   Infinite Loop Elimination (무한 루프 제거)   | [Details](https://developercommunity.visualstudio.com/t/Optimization-Levels-O1-O2-Ox-Incorrect/10478781?sort=newest) |
| MSVC | x86-64 |   Inaccurate Calculation and Comparison of Constants (상수의 부정확한 계산 및 비교)     | [Details](https://developercommunity.visualstudio.com/t/Incorrectly-compiled-comparison-and-cons/10480723?sort=newest) |
| MSVC | x86-64 |   Non-Compliance with C Standard for Hexadecimal Literal Constants (16진수 상수 리터럴 c 표준 미준수)     | [Details](https://developercommunity.visualstudio.com/t/cl-Compiler-Misinterprets-Hexadecimal-Li/10483175) |
| MSVC | x86-64 |   Omission of Stack Initialization for Local Variables (지역 변수의 스택 초기화 누락)     | [Details](https://developercommunity.visualstudio.com/t/Function-pointer-address-comparison-erro/10485960?sort=newest) |
| MSVC | x86-64 |   Compiler Crash (크래시)   | [Details](https://developercommunity.visualstudio.com/t/Internal-Compiler-Error-with-for-loop-an/10486573) |
| MSVC | x86-64 |   Compiler Crash (크래시)   | [Details](https://developercommunity.visualstudio.com/t/fatal-error-C1001:-Internal-Compiler-Err/10485991?sort=newest) |
| MSVC | x86-64 |   Sign/Unsign Extension Issue (부호 확장 문제)   | [Details](https://developercommunity.visualstudio.com/t/Signed-variable-value-extended-in-an-uns/10478879?sort=newest&q=Signed+variable+value+extended+in+an+unsigned+manner&page=3) |
| MSVC | x86-64 |   Sign/Unsign Extension Issue (부호 확장 문제)   | [Details](https://developercommunity.visualstudio.com/t/Incorrect-unsigned-extension-when-upcast/10481317?sort=newest) |
| MSVC | x86-64 | Sign/Unsign Extension Issue (부호 확장 문제) | [Details](https://developercommunity.visualstudio.com/t/Impact-of-printf-on-CL-Compiler-Optimiza/10481033?sort=newest) |
| MSVC | arm64 |    Sign/Unsign Extension Issue (부호 확장 문제)   | [Details](https://developercommunity.visualstudio.com/t/Incorrect-Assembly-Code-Generated-with-/10506096) |
| MSVC | x86-64 |   Inaccurate Computation (부정확한 연산)    | [Details](https://developercommunity.visualstudio.com/t/O2-and-Ox-Optimizations-Result-in-Incorr/10476654?sort=newest) |
| MSVC | x86-64 |   Inaccurate Computation (부정확한 연산)    | [Details](https://developercommunity.visualstudio.com/t/Integer-overflow-due-to-optimization-in/10478835?sort=newest) |
| MSVC | x86-64 |   Inaccurate Computation (부정확한 연산)    | [Details](https://developercommunity.visualstudio.com/t/Comparison-of-incorrect-register-values/10480763?sort=newest) |
| MSVC | x86-64 |   Inaccurate Computation (부정확한 연산)    | [Details](https://developercommunity.visualstudio.com/t/It-optimizes-the-and-operation-into-x/10481313) |
| MSVC | x86-64 |   Inaccurate Computation (부정확한 연산)    | [Details](https://developercommunity.visualstudio.com/t/Compiler-bug-causing-unknown-behavior/10481332?sort=newest) |