# blue_course_test2

test2 : 맵 문자열을 변환하고 출력하는 프로그램

1) 문자열을 읽어 json으로 저장하는 함수

1. arguments로 들어온 string을 slice함수를 통해 0에서부터 "," 전까지 잘라서 Number형으로 바꾼후 width 변수에 저장합니다.
2. arguments로 들어온 string을 slice함수를 통해 "," 다음부터 "\n" 전까지 잘라서 Number형으로 바꾼후 height 변수에 저장합니다.
3. arguments로 들어온 string을 slice함수를 통해 "\n"부터 끝까지 자른후 split 함수를 통해 배열로 만듭니다.
4. 그후 map 함수를 통해 만약 "\n"이 있으면 undefined로 바꾸고 "-"이 있으면 " "로 바 그 외에는 원래 값으로 return 합니다.
   undefined로 바꾼 이유는 join함수를 사용하였을때 배열의 undefined를 무시하기 때문입니다.
5. 마지막으로 join함수를 통해 배열을 값을 string으로 만들고 data변수에 저장합니다.
6. width변수와 height변수, data변수로 객체를 만들어 return 합니다.


2) 1의 json을 2차원 배열로 변환하고 해당 배열을 화면에 출력하는 함수를 작성하세요. 단 - 는 공백으로 바꾸어 출력합니다.

1. parseData함수로 부터 만든 json 객체를 arguments로 받아 split함수를 통해 배열로 만듭니다.
2. 이중 for문을 사용하여 width 만큼 반복하여 newArr 배열에 값을 넣고 한 행이 끝나면 arr배열에 해당 newArr를 넣습니다. 그후 splice함수를 사용하여 0부터 width번째 까지의 배열을 잘라내고 다시 반복하여 2차원 배열을 생성합니다.
3. 마지막으로 forEach함수를 통해 console.log로 2차원 배열의 원소를 하나씩 join함수로 string으로 만들고 console.log로 print합니다. 

html파일을 실행 시키고 콘솔을 확인하시면 테스트 값의 결과를 보여즙니다.
언어는 자바스크립트를 사용하였습니다.
