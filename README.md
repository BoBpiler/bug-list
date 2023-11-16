# Compilers Optimization Bugs reported by BoBpiler Team

이 문서는 BoBpiler 팀이 발견하고 보고한 다양한 컴파일러 최적화 관련 버그들의 모음집입니다. 각 버그는 발생한 컴파일러, 아키텍처, 버그의 유형 및 관련 링크로 구성되어 있습니다. 이 목록은 컴파일러 최적화 과정에서 발견된 잠재적인 문제들을 식별하고 연구하는 데 도움을 주기 위해 작성되었습니다.

보고된 각 버그는 연구 및 교육 목적으로 사용될 수 있으며, 해당 분야의 전문가들이 문제를 해결하고, 소프트웨어 개발 과정에서 발생할 수 있는 유사한 문제를 예방하는 데 기여할 수 있습니다.


| Compiler | Arch | Bug Type | Link |
| --- | --- | --------------------------- | ---- |
| gcc | s390x |     부정확한 연산    | https://gcc.gnu.org/bugzilla/show_bug.cgi?id=112112 |
| gcc | s390x |     부정확한 연산    | https://gcc.gnu.org/bugzilla/show_bug.cgi?id=112274 |
| gcc | s390x |     부정확한 연산    | https://gcc.gnu.org/bugzilla/show_bug.cgi?id=112329 |
| llvm | x86-64 |   무한 루프 제거    | https://github.com/llvm/llvm-project/issues/66307 |
| llvm | arm64 |    포인터 역참조 생략   | https://github.com/llvm/llvm-project/issues/69294 |
| llvm | riscv |    부호 확장 문제   | https://github.com/llvm/llvm-project/issues/68855 |
| llvm | powerpc64 |    부호 확장 문제   | https://github.com/llvm/llvm-project/issues/71030 |
| llvm | mips64el |     부정확한 연산    | https://github.com/llvm/llvm-project/issues/69328 |
| llvm | mips64 |   부정확한 연산    | https://github.com/llvm/llvm-project/issues/70495 |
| llvm | s390x |    부정확한 연산    | https://github.com/llvm/llvm-project/issues/72018 |
| MSVC | arm64 |    부정확한 연산    | https://developercommunity.visualstudio.com/t/C-ARM64-Optimization-Bug/10503910 |
| MSVC | arm64 |    부정확한 연산    | https://developercommunity.visualstudio.com/t/Inconsistent-Outputs-in-ARM64-C-Progra/10505191 |
| MSVC | arm64 |    부정확한 연산    | https://developercommunity.visualstudio.com/t/ARM64-MSVC-Compiler-Optimization-Leads-t/10508262 |
| MSVC | arm64 |    부정확한 연산    | https://developercommunity.visualstudio.com/t/MSVC-ARM64-Compiler-Incorrectly-Optimize/10510611 |
| MSVC | x86-64 |   부정확한 인라인 호출 순서    | https://developercommunity.visualstudio.com/t/O1-Optimization-Leads-to-Incorrect-Funct/10469220?sort=newest |
| MSVC | x86-64 |   다른 변수 주소 동일 인식     | https://developercommunity.visualstudio.com/t/Memory-reference-error-due-to-excessive/10477735?sort=newest&page=1 |
| MSVC | x86-64 |   무한 루프 제거   | https://developercommunity.visualstudio.com/t/Optimization-Levels-O1-O2-Ox-Incorrect/10478781?sort=newest |
| MSVC | x86-64 |   상수의 부정확한 계산 및 비교     | https://developercommunity.visualstudio.com/t/Incorrectly-compiled-comparison-and-cons/10480723?sort=newest |
| MSVC | x86-64 |   16진수 상수 리터럴 c 표준 미준수     | https://developercommunity.visualstudio.com/t/cl-Compiler-Misinterprets-Hexadecimal-Li/10483175 |
| MSVC | x86-64 |   지역 변수의 스택 초기화 누락     | https://developercommunity.visualstudio.com/t/Function-pointer-address-comparison-erro/10485960?sort=newest |
| MSVC | x86-64 |   크래시   | https://developercommunity.visualstudio.com/t/Internal-Compiler-Error-with-for-loop-an/10486573 |
| MSVC | x86-64 |   크래시   | https://developercommunity.visualstudio.com/t/fatal-error-C1001:-Internal-Compiler-Err/10485991?sort=newest |
| MSVC | x86-64 |   부호 확장 문제   | https://developercommunity.visualstudio.com/t/Signed-variable-value-extended-in-an-uns/10478879?sort=newest&q=Signed+variable+value+extended+in+an+unsigned+manner&page=3 |
| MSVC | x86-64 |   부호 확장 문제   | https://developercommunity.visualstudio.com/t/Incorrect-unsigned-extension-when-upcast/10481317?sort=newest |
| MSVC | x86-64 | 부호 확장 문제 | https://developercommunity.visualstudio.com/t/Impact-of-printf-on-CL-Compiler-Optimiza/10481033?sort=newest |
| MSVC | arm64 |    부호 확장 문제   | https://developercommunity.visualstudio.com/t/Incorrect-Assembly-Code-Generated-with-/10506096 |
| MSVC | x86-64 |   부정확한 연산    | https://developercommunity.visualstudio.com/t/O2-and-Ox-Optimizations-Result-in-Incorr/10476654?sort=newest |
| MSVC | x86-64 |   부정확한 연산    | https://developercommunity.visualstudio.com/t/Integer-overflow-due-to-optimization-in/10478835?sort=newest |
| MSVC | x86-64 |   부정확한 연산    | https://developercommunity.visualstudio.com/t/Comparison-of-incorrect-register-values/10480763?sort=newest |
| MSVC | x86-64 |   부정확한 연산    | https://developercommunity.visualstudio.com/t/It-optimizes-the-and-operation-into-x/10481313 |
| MSVC | x86-64 |   부정확한 연산    | https://developercommunity.visualstudio.com/t/Compiler-bug-causing-unknown-behavior/10481332?sort=newest |