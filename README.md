
REAMDE.md(markdown)에서 사용하는 Markdown 문법을 정리한다.

What is the Markdown ?
----------------------

Markdown은 웹상에 텍스트를 몇가지의 제어문자들을 이용해서 적절한 형태로 표현하는 방법입니다.
TEXT를 BOLD 또는 ITALIC 형태의 글꼴로 설정하거나 이미지를 추가하거나 목록(LIST)를 작성, 문서의 표시를 제어한다.
대부분, # 또는 *처럼 알파벳이 아닌 몇몇 문자들은 그냥 일반 텍스트로 본다.
초보자라면 
여기 사이트[MARKDOWN-BASICS](https://help.github.com/articles/markdown-basics) 통해서 기초부터 볼수 있다.
3분만 투자하면 MASTER 할수 있는 사이트[MASTER-MARKDOWN](http://guides.github.com/overviews/mastering-markdown/#intro)
도 소개한다.

GitHub에서는 전통적인 Markdown 문법과 GFM(GitHub Flavored Markdown)이라고하는 GitHub 에서 사용하는 Markdown과의
차이점을 정리한 사이트[GITHUB-FAVORED-MARKDOWN](https://help.github.com/articles/github-flavored-markdown)에서 확인이 가능하다.


#문법가이드

###라인 구분 
에디터 상에서 아래와 같이 입력해도 옆으로 붙어서 표시 될것이다.<BR>

(VI 에디터 or GitHub Code상의 입력)
```
This is First Line
This is Second Line
```

(WEB에서의 출력 or Preview 출력)
```
This is First Line This is Second Line
```

단지 에디터상의 라인 구분은 출력에서 SPACE으로 표시된다. 일반적으로 \\n과 같은 다음 라인으로 TEXT를 출력하고 싶다면,
에디터 상에서 아래와 같이 TEXT 끝에 \<BR\>  or \<br\>을 추가한다.

(VI 에디터 or GitHub Code상의 입력)
```
This is First Line<BR>
This is Second Line
```
(WEB에서의 출력 or Preview 출력)
```
This is First Line 
This is Second Line
```

###단락 구분
단락(문단)구분은 빈줄을 에디터에서 TEXT 와 TEXT 사이에 추가하므로 할 수 있다.

(VI 에디터 or GitHub Code상의 입력)
```
This is First Paragraphs

This is Second Paragraphs 
```
(WEB에서의 출력 or Preview 출력)
```
This is First Paragraphs

This is Second Paragraphs 
```

###해더 추가
단락 시작 전에 해당 단락의 내용을 규정하는 HEADER 폼을 추가하고 싶다면, 글자 앞에 하나 이상의 \# 을 추가하면 된다.<BR>
\#의 수에 따라 글자의 크기를 조절할 수 있다.

(VI 에디터 or GitHub Code상의 입력)
```
#가장 큰 HEADING TEXT
##두번째 큰 HEADING TEXT
. . .
######여섯번째로 큰 HEADING TEXT
```
(WEB에서의 출력 or Preview 출력)

---------------------------------
#가장 큰 헤더 TEXT 
##두번째 큰 HEADING TEXT
######여섯번째로 큰 HEADING TEXT
---------------------------------

###인용 블럭
문자열 앞에 \>를 주면 인용 블럭을 표시 할 수있다.

(VI 에디터 or GitHub Code상의 입력)
```
푸시킨이 말 중에 : 
> 삶이 그대를 속일지라고 노여워 ....
```
(WEB에서의 출력 or Preview 출력)

푸시킨이 말 중에 : 
> 삶이 그대를 속일지라고 노여워 ....

###글꼴 스타일

문자열 앞과 끝에 \* 을 넣으면 italic style이 되고, 문자열 앞과 끝에  \*\*  넣으면 bold style로 된다.

(VI 에디터 or GitHub Code상의 입력)
```
*이텔릭체*
**볼드체**
```
(WEB에서의 출력 or Preview 출력)

*이텔릭체*<BR>
**볼드체**

또한 **BOLD** 와 *ITALIC*을 한문장에서 같이 사용할 수있다. 한문장에서 표현 할때는 


**Everyone _must_ attend the meeting at 5 o'clock today.** <BR>
*Everyone _must_ attend the meeting at 5 o'clock today.*
#Syntax Highlighting

####1.C소스 Syntax Highlighting하는 방법.
아래와 같이 소스에 해당 언어의 SYNTAX HIGHLIGHTING을 주고 싶으면 처음 시작하는 \`\`\`끝에 C를 추가하면 된다.
```C
int main(void)
{
  printf("Hello World\n");
  return 0;
}
```









