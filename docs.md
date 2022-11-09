---
layout: default
permalink: portfolio
---

# 비트 마스킹 정리표

| `연산` | `사용 예시` |
| `공집합과 꽉 찬 집합 구하기`| `A = 0; / A = (1 << 10) - 1;` |
| `원소 추가 `| `A |= (1 << k);` |
| `원소 삭제` |`A &= ~(1 << k);` |
| `원소의 포함 여부 확인` | `if(A & (1 << k))` |
| `원소의 토글(toggle)` | `A ^= (1 << k);` |
| `두 집합에 대해서 연산`| `A | B → A와 B의 합집합` |
`A & B → A와 B의 교집합`
`A & (~B) → A에서 B를 뺀 차집합`
`A ^ B → A와 B중 하나에만 포함된 원소들의 집합 ` |
|`집합의 크기 구하기`| `int bitCount(int A){ if(A == 0) return 0; return A%2 + bitCount(A / 2); }`|

|`[내장 명령어]` |
`gcc/g++ → __builtin_popcount(A)`
`visual C++ → __popcnt(A)`
`Java → Integer.bitCount(A)` |
|`최소 원소 찾기` | `int first = A & (-A);` |
|`최소 원소 지우기` | `A &= (A - 1);` |
|`모든 부분 집합 순회하기` | `for (int subset = A ; subset ; subset = ((subset - 1) & A)){ }` |

```

```
