# UCPC 디스크립션 작성 및 포매팅 컨벤션

이 컨벤션에서 다음의 용어는 RFC 2119에서 규정된 각각의 용어에 대응됩니다.

* "합니다": "MUST". 어떤 상황에서든 반드시 준수해야 합니다.
* "하지 않습니다": "MUST NOT". 어떤 상황에서든 절대 해서는 안 되는 사항입니다.
* "하는 것을 권장합니다": "SHOULD". 특별한 상황에서 그렇게 하지 않을 정당한 이유가 있으면 무시할 수 있으나, 그렇게 할 경우 신중한 고려가 필요합니다.
* "하지 않는 것을 권장합니다": "SHOULD NOT". 특별한 상황에서 그렇게 할 정당한 이유가 있으면 무시할 수 있으나, 그렇게 할 경우 신중한 고려가 필요합니다.
* "해도 됩니다": "MAY".

## 공통

### 문장

1. 모든 문제의 디스크립션은 맞춤법을 지키도록 작성하려고 하는 것을 권장합니다. 단, 극히 예외적인 상황에서 일부러 맞춤법을 어기려는 컨셉의 문제에서는 그렇게 하지 않아도 됩니다. 또한, 맞춤법을 지키지 않는 표현이 맞춤법을 지키는 표현보다 매우 널리 사용되는 경우에도 맞춤법을 지키지 않아도 됩니다.

   **예 1)** 영어 알파벳의 열여덟 번째 자모 이름인 'R'을 한글로 적을 때 '아르'로 적기 때문에, 이를 기준으로 뒤따르는 조사로 '와'를 사용하는 것이 올바른 맞춤법입니다. 하지만, 'R'을 '알'이라고 읽고 조사로 '과'를 사용하는 것이 널리 통용되므로, 'R과'와 같이 작성해도 됩니다.

   **예 2)** 외래어표기법에 따르면 'damage'는 '대미지'와 같이 적습니다. 단, '데미지'라는 표현이 널리 통용되기 때문에 '데미지'와 같이 작성해도 됩니다. 

2. 디스크립션의 모든 문장을 짧고 간결하게 작성하는 것을 권장합니다. 단, 참가자의 독해를 일부러 어렵게 하려는 컨셉의 문제에서는 그렇게 하지 않아도 됩니다.

3. 문장에서 괄호를 사용하지 않는 것을 권장합니다.

4. 문제 해결에 직접적으로 필요하지 않은 정보를 너무 많이 제공하지 않는 것을 권장합니다.

5. 수학 기호들은 문제와 참가자 수준에 맞도록 사용하는 것을 권장합니다. 디스크립션이 너무 길고, 수학 기호를 사용함으로서 디스크립션을 훨씬 더 간결하게 만들 수 있다면, 디스크립션이나 노트, 힌트 등에 해당 기호에 대한 정의를 제공합니다.

### 변수

1. 한 번만 입력받는 변수는 대문자, 이외의 다른 변수는 소문자로 정하는 것을 권장합니다.

   **예 1)** 프로그램의 입력은 *T*개의 테스트 데이터로 이루어져 있다. *T*는 입력의 맨 첫 줄에 주어진다.
   
   **예 2)** 이어서 *E*개의 줄에 걸쳐 간선을 이루는 두 점 *a*와 *b*가 공백으로 구분되어 주어진다.
   
2. 변수의 범위 제한은 **[입력] 섹션**에서 해당 상수나 변수가 처음 등장하는 위치에 적는 것을 권장합니다. 가능한 경우, 제한은 부등호를 사용한 수식으로 적는 것을 권장합니다. 범위 제한을 여러 개 적을 경우에는, 세미콜론(;)으로 구분합니다.

   **예 1)** 첫째 줄에 세 수 *A*, *B*, *C*가 공백으로 구분되어 주어진다. (1 ≤ *A*, *B* ≤ 1 000 000; 1 ≤ *C* ≤ 10<sup>9</sup>)
   
   **예 2)** 첫째 줄에 블록을 놓은 횟수 *N*(1 ≤ *N* ≤ 10 000)이 주어진다.
   
3. 수는 3자리씩 공백으로 끊어 적습니다. 수가 10<sup>7</sup>보다 크거나 같은 경우 지수를 이용해 표시하는 것을 권장합니다. 과학적 표기법으로 표현하는 것이 의미가 없는 수는 풀어서 표기하지만, 특별한 의미를 가진 경우 괄호 안에 넣어 등호(=) 기호와 함께 표기합니다. 수 뒤의 조사는 수를 표시된 대로 한국어로 읽었을 때를 기준으로 붙입니다.

   **예 1)** 전체 경우의 수가 10<sup>7</sup>(십의 일곱제**곱**)을 넘지 않음을 증명할 수 있다.
   
   **예 2)** 첫 반례는 906 150 257(...이백오십**칠**)로 알려져 있다.
   
   **예 3)** 결과를 1 000 000 007(= 10<sup>9</sup> + 7)로 나눈 나머지를 출력한다. 이 수는 소수이다.
   
   **예 4)** 결과를 998 244 353(= 119 &times; 2<sup>23</sup> + 1)으로 나눈 나머지를 출력한다. 이 수는 소수이다.
   
4. 수열 인덱스는 1부터 시작하는 것으로 정하는 것을 권장합니다.

5. 변수의 제한에서 '자연수'라는 단어는 사용하지 않습니다. 문맥에 따라 '양의 정수' 혹은 '음이 아닌 정수'로 바꿔 사용합니다.

### 입력과 출력

1. 입출력 형식은 코드로 짜기 너무 어렵지 않도록 정합니다.
   
   1. 특히 EOF로 입력의 끝을 명시하는 것은 피하는 것을 권장합니다.
   2. 입력받아야 하는 문자열이 공백을 포함할 수 있는 상황도 피하는 것을 권장합니다.
   
2. 입출력 형식을 예를 들어 명시하는 경우, 예시는 본문과 명확히 구분될 수 있도록 포매팅을 다르게 합니다.

   **예 1)** 가능한 경우가 있으면 `YES`, 없으면 `NO`를 출력한다.
   
   **예 2)** 쿼리는 `a i j k`와 같은 형식으로 들어온다.
   
3. 한 줄에 여러 개의 정보를 작성하는 경우, 입력 형식에 공백으로 구분하였는지 아닌지를 명시합니다. 

   **예 1)** 첫째 줄에 가로 길이 *N*과 세로 길이 *M*이 공백으로 구분되어 주어진다.

   **예 2)** 둘째 줄에 높이를 나타내는 한 자리 정수 *N*개가 공백 없이 주어진다.

   **예 3)** 셋째 줄에 가격을 나타내는 *A*개의 정수가 공백으로 구분되어 주어진다.

### 문제 예시와 예제

1. 문제 예시는 디스크립션에 적기보다는 **[예제 입력과 출력] 섹션**을 활용합니다.
2. 필요한 경우 그림을 삽입해 참가자의 이해를 돕도록 하는 것을 권장합니다.
3. 예제 입력으로는 참가자가 직접 생각해 볼 수 있는 수준의 작은 예제를 적어도 하나 제공하는 것을 권장합니다.

# 포매팅

## TeX

1. 모든 변수와 기수 등은 math mode로 작성해야 합니다. 서수는 text mode로 작성해도 됩니다.

   | 올바른 예                                                    | 잘못된 예                                                    |
   | ------------------------------------------------------------ | ------------------------------------------------------------ |
   | `프로그램의 입력은 $T$개의 테스트 데이터로 이루어져 있다.`   | `프로그램의 입력은 T개의 테스트 데이터로 이루어져 있다.`     |
   | `첫째 줄에 $A$와 $B$가 주어진다. $(1\leq A,B\leq 10^5)$`     | `첫째 줄에 A와 B가 주어진다. (1 ≤ A, B ≤ 10^5)`              |
   | `결과를 $998\,244\,353$으로 나눈 나머지를 출력한다.`         | `결과를 998 244 353으로 나눈 나머지를 출력한다.`             |
   | `예를 들면 102호 방보다는 301호 방을 더 선호하는데, 102호는 거리 $2$만큼 걸어야 하지만 301호는 거리 $1$만큼만 걸으면 되기 때문이다.` | `예를 들면 102호 방보다는 301호 방을 더 선호하는데, 102호는 거리 2만큼 걸어야 하지만 301호는 거리 1만큼만 걸으면 되기 때문이다.` |

2. 변수 등을 나열하는 쉼표 바로 뒤에는 공백이 <u>들어오지 않아야</u> 합니다. HTML 섹션의 포매팅 컨벤션과 다름에 유의해 주세요. (TeX는 math mode에서 기본적으로 comma 뒤에 약간의 공백을 삽입합니다.)

   | 올바른 예              | 잘못된 예                    |
   | ---------------------- | ---------------------------- |
   | `$1\leq A,B\leq 10^5$` | `$1\leq A,\,B\leq 10^5$`     |
   | `$A_1,A_2,\cdots,A_n$` | `$A_1,\,A_2,\,\cdots,\,A_n$` |

3. 식의 끝이 문장의 끝이라면 마침표를 붙입니다.

   | 올바른 예                                                    | 잘못된 예                                                   |
   | ------------------------------------------------------------ | ----------------------------------------------------------- |
   | `$B_i$는 아래 식과 같이 계산된다. \[B_i=\sum_{j=0}^i A_i.\]` | `$B_i$는 아래 식과 같이 계산된다. \[B_i=\sum_{j=0}^i A_i\]` |

4. 괄호에는 \left, \right을 붙이는 것을 권장합니다. 집합을 표현할 때 문자 ‘|’는 \mid으로 표현합니다.

   | 올바른 예                                     | 잘못된 예                          |
   | --------------------------------------------- | ---------------------------------- |
   | `$A_i=\left(\int_0^i x^a+bx\sin x dx\right)$` | `$A_i=(\int_0^i x^a+bx\sin x dx)$` |

5. 나열된 제한을 구분하는 `;` 문자 뒤에서 수식을 닫습니다. 특히 MathJax 렌더러 환경에서, 입력 제한을 줄 때 괄호 `(`, `)`도 수식 안에 포함하는 것을 권장합니다. 좁은 화면에서 제한이 잘 표시되도록 합니다. 

      | 올바른 예                                            | 잘못된 예                                          |
   | ---------------------------------------------------- | -------------------------------------------------- |
   | `$(1 \le A, B \le 1\,000\,000;$ $1 \le C \le 10^9)$` | `($1 \le A, B \le 1\,000\,000; 1 \le C \le 10^9$)` |
   
6. 순서가 있는 리스트는 enumerate, 순서가 없는 리스트는 itemize를 사용합니다.

7. sin, cos, max, lim 등은 그대로 적지 말고 각각의 함수에 맞는 operator를 사용하도록 합니다. 각각 \sin, \cos, \max, \lim 등입니다.

8. ‘...’ 기호는 그대로 적지 말고 \cdots를 사용하도록 합니다.

9. 수식 안에 텍스트를 써야 할 경우에는 \text를 사용하도록 합니다.

10. 인라인 수식에서 \displaystyle(\dfrac 포함)을 사용하지 않는 것을 권장합니다. 인라인 수식이 너무 복잡해 문제의 가독성을 해칠 경우에는, 문맥을 적절히 수정하여 블록 수식으로 적는 것을 권장합니다.

## HTML

1. 모든 변수는 기울임꼴으로 표시합니다. 숫자와 연산자는 어떤 경우에도 기울임꼴로 표시하지 않습니다. 필요에 따라 벡터, 행렬, 텐서의 경우, 굵은 기울임꼴로 표시해도 됩니다.

   | 올바른 예                                                | 잘못된 예                                                    |
   | -------------------------------------------------------- | ------------------------------------------------------------ |
   | 프로그램의 입력은 *T*개의 테스트 데이터로 이루어져 있다. | 프로그램의 입력은 T개의 테스트 데이터로 이루어져 있다.       |
   | 행렬 ***A***, ***B***와 벡터 ***v***가 주어진다.         | 행렬 A, B와 벡터 v가 주어진다.                               |
   | arcsin *x*의 값을 출력한다.                              | *arcsin* *x*의 값을 출력한다.                                |
   | *A*<sub>1</sub>, *A*<sub>2</sub>, ..., *A*<sub>*n*</sub> | *A*<sub>*1*</sub>, *A*<sub>*2*</sub>, ..., *A*<sub>*n*</sub> |

2. 연산자와 문자, 혹은 연산자와 수 사이에는 띄어쓰기를 반드시 포함해야 합니다.

   | 올바른 예                                                    | 잘못된 예                                             |
   | ------------------------------------------------------------ | ----------------------------------------------------- |
   | 10<sup>9</sup> + 7                                           | 10<sup>9</sup>+7                                      |
   | *A* + *B*                                                    | A+B                                                   |
   | *a*<sub>1</sub> + *a*<sub>2</sub> + … + *a*<sub>*i* − 1</sub> | *a*<sub>1</sub>+*a*<sub>2</sub>+…+*a*<sub>*i*−1</sub> |

3. 변수 등을 나열하는 쉼표 바로 뒤에는 공백이 <u>있어야</u> 합니다. TeX 섹션의 포매팅 컨벤션과 다름에 유의해 주세요.

4. 유니코드에 사용 가능한 기호가 있다면, 올바른 기호를 선택해서 사용해야 합니다.

   | 올바른 예                           | 잘못된 예               |
   | ----------------------------------- | ----------------------- |
   | &minus; `&minus;`                   | -                       |
   | &times; `&times;`                   | *                       |
   | &mldr; `&mldr;`                     | ...                     |
   | &le; `&le;`                         | &lt;=                   |
   | &ge; `&ge;`                         | &gt;=                   |
   | &ne; `&ne;`                         | !=                      |
   | &rightarrow; `&rightarrow;`         | -&gt;                   |
   | &Rightarrow; `&Rightarrow;`         | =&gt;                   |
   | &leftarrow; `&leftarrow;`           | &lt;-                   |
   | &Leftarrow; `&Leftarrow;`           | &lt;=                   |
   | &leftrightarrow; `&leftrightarrow;` | &lt;-&gt;               |
   | &Leftrightarrow; `&Leftrightarrow;` | &lt;=&gt;               |
   | &equiv; `&equiv;`                   | ===                     |
   | &cong; `&cong;`                     | ~=                      |
   | &sim; `&sim;`                       | ~                       |
   | &lsquo;&rsquo; `&lsquo;&rsquo;`     | '' (리터럴이 아닌 경우) |
   | &ldquo;&rdquo; `&ldquo;&rdquo;`     | "" (리터럴이 아닌 경우) |
   | &#x20a9; `&#x20a9;`                 | \ (리터럴이 아닌 경우)  |

5. TeX 렌더 엔진을 사용해야 할 경우, 일관성을 위해 콘테스트 전체의 모든 문제에 사용합니다. 이 경우 모든 수식은 TeX 섹션의 포매팅 컨벤션을 따라야 합니다.

수식의 HTML 변환을 도와주는 [BOJ 디스크립션 툴](https://solved-ac.github.io/boj-description-converter/)을 사용해도 됩니다.

이 컨벤션에 없는 HTML 포매팅 사항들에 관련해서는 [BOJ Stack의 요구사항](https://stack.acmicpc.net/guide/problem)을 따르도록 합니다.
