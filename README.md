# Compiler_Parser
using yacc

1. 실습 환경 : ubuntu 16.04

2.  수정
	1) globals.h
		yacc 폴더에 있는 걸 수정
	2) main.c
	 	Parse 사용 위해 상수 수정
	3) Makefile
		커맨드로 안치고 한번에 작동하도록 
	  	y.tab.o 등록, 컴파일 에러 나서 y.tab.o, lex.yy.o, main.o, util.o, 				symtab.o 이 5개만 타겟으로 등록
	4) util.c, util.h 
		BNF에서 고친 문법에 따라 함수 넣기. Tree 출력 가능하게 수정
	5) cminus.y
		이 것 또한 tiny.y를 가져와 수정

3. 실행 결과
	1) 실행 방법  make cminus, ./cminus test.cm
