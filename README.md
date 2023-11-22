# 컴파일러 최적화 버그 제보
## List of Compiler Optimization Bugs Reported by BoBpiler Team

이 문서는 BoBpiler 팀이 [BoBpiler 퍼저](https://github.com/BoBpiler/BoBpiler-Fuzzer)를 사용하여 발견하고 보고한 다양한 컴파일러의 최적화 버그들을 모아놓은 목록입니다. 각 컴파일러, 아키텍처, 버그 유형 및 상세 링크를 포함하고 있습니다. 이러한 버그 리포트는 해당 분야의 전문가들이 문제를 해결하고 소프트웨어 개발 과정에서 발생할 수 있는 유사한 문제와 잠재적인 보안 취약점을 예방하는 데 기여할 수 있습니다.

This document contains a compilation of various compiler optimization bugs discovered and reported by the BoBpiler Team using the [BoBpiler Fuzzer](https://github.com/BoBpiler/BoBpiler-Fuzzer). It includes the compiler, architecture, type of bug, and a link to further details. Each bug report can assist experts in resolving issues, thereby helping to prevent similar issues and potential security vulnerabilities in the software development process.

GCC 컴파일러 관련 버그는 Bugzilla에서, LLVM 컴파일러 관련 버그는 Git Issue에서 개발자들과 소통 중입니다. MSVC의 경우, 개발자들이 버그를 확인하고, 상태를 'Under Consideration' 또는 'Under Investigation' 등으로 분류하여 봇을 통해 공지합니다.

Bugs related to the GCC compiler are being communicated with developers on Bugzilla, while those related to the LLVM compiler are discussed on Git Issues. For MSVC, developers acknowledge bugs and categorize their status as 'Under Consideration' or 'Under Investigation', which is then announced through bots.

### Explanation of Bug Status / 버그 상태 설명
**GCC (Bugzilla):** 
- 버그질라에서는 버그 상태가 다양하게 표시될 수 있지만, 여기서는 간단하게 `Open`으로 표기했습니다. 이는 버그가 인식되었고 해결을 기다리는 상태를 의미합니다.
- Although Bugzilla shows various statuses for bugs, here we have simplified it as `Open`. This indicates that the bug has been recognized and is awaiting resolution.

**LLVM (Git Issue):** 
- 버그 상태는 `Open` 또는 `Closed (Fixed)`로 표시됩니다. `Open`는 버그가 아직 해결되지 않았음을, `Closed (Fixed)`는 버그가 해결되었음 혹은 해당 이슈가 종료되었음을 나타냅니다.
- The bug status is designated as `Open` or `Closed (Fixed)`. `Open` signifies that the bug is still pending resolution, while `Closed (Fixed)` indicates that the bug has been resolved or the issue has been closed.

**MSVC:** 
- 버그 상태는 `UC (Under Consideration)`, `UI (Under Investigation)`, 또는 `Fixed` 등으로 표시됩니다. [`UC`](https://developercommunity.visualstudio.com/t/Comparison-of-incorrect-register-values/10480763?sort=newest)는 MSVC 팀이 문제를 인지하고 내부적으로 버그로 등록했으며, 수정을 고려 중임을 나타냅니다. 문제가 내부적으로 해결되면, 상태는 `Fixed in Pending Release`로 변경됩니다. 수정사항이 Visual Studio의 발표된 버전에 포함되면, 상태는 `Fixed`로 업데이트됩니다.
- The bug status is categorized as `UC (Under Consideration)`, `UI (Under Investigation)`, or `Fixed`. [`UC`](https://developercommunity.visualstudio.com/t/Comparison-of-incorrect-register-values/10480763?sort=newest) indicates that the MSVC team has acknowledged the issue and created an internal bug to track it, and they are considering fixing it. Once the bug is resolved internally, the status will be updated to `Fixed in Pending Release`. After the fix is included in the released version of Visual Studio, the status will be changed to `Fixed`.
![Under Consideration](png/Under_Consideration.png)

---
| Compiler | Arch | Bug Type | Status | Link |
| --- | --- | --------------------------- | ---- | ---- |
| GCC | S390x |     Inaccurate Computation (부정확한 연산)    | Open | [Details](https://gcc.gnu.org/bugzilla/show_bug.cgi?id=112112) |
| GCC | S390x |     Inaccurate Computation (부정확한 연산)    | Open | [Details](https://gcc.gnu.org/bugzilla/show_bug.cgi?id=112274) |
| GCC | S390x |     Inaccurate Computation (부정확한 연산)    | Open | [Details](https://gcc.gnu.org/bugzilla/show_bug.cgi?id=112329) |
| LLVM | Arm64 |    Pointer Dereference Omission (포인터 역참조 생략)   | Open | [Details](https://github.com/llvm/llvm-project/issues/69294) |
| LLVM | Risc-v |    Sign/Unsign Extension Issue (부호 확장 문제)   | Closed (Fixed) | [Details](https://github.com/llvm/llvm-project/issues/68855) |
| LLVM | Powerpc64 |    Sign/Unsign Extension Issue (부호 확장 문제)   | Open | [Details](https://github.com/llvm/llvm-project/issues/71030) |
| LLVM | Mips64el |     Inaccurate Computation (부정확한 연산)    | Open | [Details](https://github.com/llvm/llvm-project/issues/69328) |
| LLVM | Mips64 |   Inaccurate Computation (부정확한 연산)    | Open | [Details](https://github.com/llvm/llvm-project/issues/70495) |
| LLVM | S390x |    Inaccurate Computation (부정확한 연산)    | Open | [Details](https://github.com/llvm/llvm-project/issues/72018) |
| MSVC | Arm64 |    Inaccurate Computation (부정확한 연산)    | UC | [Details](https://developercommunity.visualstudio.com/t/C-ARM64-Optimization-Bug/10503910) |
| MSVC | Arm64 |    Inaccurate Computation (부정확한 연산)    | UC | [Details](https://developercommunity.visualstudio.com/t/Inconsistent-Outputs-in-ARM64-C-Progra/10505191) |
| MSVC | Arm64 |    Inaccurate Computation (부정확한 연산)    | UC | [Details](https://developercommunity.visualstudio.com/t/ARM64-MSVC-Compiler-Optimization-Leads-t/10508262) |
| MSVC | Arm64 |    Inaccurate Computation (부정확한 연산)    | UC | [Details](https://developercommunity.visualstudio.com/t/MSVC-ARM64-Compiler-Incorrectly-Optimize/10510611) |
| MSVC | X86-64 |   Incorrect Inline Call Order (부정확한 인라인 호출 순서)    | UC | [Details](https://developercommunity.visualstudio.com/t/O1-Optimization-Leads-to-Incorrect-Funct/10469220?sort=newest) |
| MSVC | X86-64 |   Misidentification of Different Variable Addresses (다른 변수 주소 동일 인식)     | UC | [Details](https://developercommunity.visualstudio.com/t/Memory-reference-error-due-to-excessive/10477735?sort=newest&page=1) |
| MSVC | X86-64 |   Infinite Loop Elimination (무한 루프 제거)   | UC | [Details](https://developercommunity.visualstudio.com/t/Optimization-Levels-O1-O2-Ox-Incorrect/10478781?sort=newest) |
| MSVC | X86-64 |   Inaccurate Calculation and Comparison of Constants (상수의 부정확한 계산 및 비교)     | UC | [Details](https://developercommunity.visualstudio.com/t/Incorrectly-compiled-comparison-and-cons/10480723?sort=newest) |
| MSVC | X86-64 |   Non-Compliance with C Standard for Hexadecimal Literal Constants (16진수 상수 리터럴 c 표준 미준수)     | UC | [Details](https://developercommunity.visualstudio.com/t/cl-Compiler-Misinterprets-Hexadecimal-Li/10483175) |
| MSVC | X86-64 |   Omission of Stack Initialization for Local Variables (지역 변수의 스택 초기화 누락)     | UC | [Details](https://developercommunity.visualstudio.com/t/Function-pointer-address-comparison-erro/10485960?sort=newest) |
| MSVC | X86-64 |   Compiler Crash (크래시)   | UC | [Details](https://developercommunity.visualstudio.com/t/Internal-Compiler-Error-with-for-loop-an/10486573) |
| MSVC | X86-64 |   Compiler Crash (크래시)   | UC | [Details](https://developercommunity.visualstudio.com/t/fatal-error-C1001:-Internal-Compiler-Err/10485991?sort=newest) |
| MSVC | X86-64 |   Sign/Unsign Extension Issue (부호 확장 문제)   | UI | [Details](https://developercommunity.visualstudio.com/t/Signed-variable-value-extended-in-an-uns/10478879?sort=newest&q=Signed+variable+value+extended+in+an+unsigned+manner&page=3) |
| MSVC | X86-64 |   Sign/Unsign Extension Issue (부호 확장 문제)   | UC | [Details](https://developercommunity.visualstudio.com/t/Incorrect-unsigned-extension-when-upcast/10481317?sort=newest) |
| MSVC | X86-64 | Sign/Unsign Extension Issue (부호 확장 문제) | UC | [Details](https://developercommunity.visualstudio.com/t/Impact-of-printf-on-CL-Compiler-Optimiza/10481033?sort=newest) |
| MSVC | Arm64 |    Sign/Unsign Extension Issue (부호 확장 문제)   | UC | [Details](https://developercommunity.visualstudio.com/t/Incorrect-Assembly-Code-Generated-with-/10506096) |
| MSVC | X86-64 |   Inaccurate Computation (부정확한 연산)    | UC | [Details](https://developercommunity.visualstudio.com/t/O2-and-Ox-Optimizations-Result-in-Incorr/10476654?sort=newest) |
| MSVC | X86-64 |   Inaccurate Computation (부정확한 연산)    | UC | [Details](https://developercommunity.visualstudio.com/t/Integer-overflow-due-to-optimization-in/10478835?sort=newest) |
| MSVC | X86-64 |   Inaccurate Computation (부정확한 연산)    | UC | [Details](https://developercommunity.visualstudio.com/t/Comparison-of-incorrect-register-values/10480763?sort=newest) |
| MSVC | X86-64 |   Inaccurate Computation (부정확한 연산)    | UC | [Details](https://developercommunity.visualstudio.com/t/It-optimizes-the-and-operation-into-x/10481313) |
| MSVC | X86-64 |   Inaccurate Computation (부정확한 연산)    | Fixed | [Details](https://developercommunity.visualstudio.com/t/Compiler-bug-causing-unknown-behavior/10481332?sort=newest) |