# hellowold
First  repository project

#문자열
sentence = '나는 소년입니다'
print(sentence)
sentence2= '파이썬은 쉬워요'
print(sentence2)
sentence3="""
나는 소년이고,
파이썬은 쉬워요
"""
print(sentence3)

#슬라이싱
jumin="040124-4830612"
print(jumin[7]) #성별
print(jumin[0:2]) #연
print(jumin[2:6]) #월일
print(jumin[:6]) #생년월일
print(jumin[7:]) #7번째 자리에서 부터 끝까지
print(jumin[-7:]) #뒤에서 부터

#문자열 처리 함수
python = "Python is Amazing"
print(python.lower())
print(python.upper())
print(python[0].isupper())
print(len(python)) #글자수(길이)
print(python.replace("Python" , "Java"))
index = python.index("n")
print(index) #n이 몇번째 자리에 위치해 있는지
index = python.index("n", index +1)
print(index) #첫번째 n자리에서(5)+!을 한 6번째 자리 위치 다음에서의 n의 자리
print(python.find("Java"))  # 두 예시 모두 오류 이지만 파인드는 -1값을, 인덱스는 오류를 냄
#print(python.index("Java"))
print(python.count("n")) #n의 갯수
print(python.find("python")) #index의 다른 방법이지 않을까?
print(python.find("n")) # 맞네,  이것 또한 n이 위치한 자리를 알려줌

#문자열포맷
print("a" + "b")
print("a" , "b")
# 방법1)
print("나는 %d살 입니다" %20)
print("나는 %s을 졸아해요" %"파이썬")
print("APPLE은 %c로 시작해요" %"A")
#모든 항목에 %S 사용가능
print("나는 %s살 입니다" %20)
print("APPLE은 %s로 시작해요" %"A")
print("나는 %s색과 %s색을 좋아해요"%("파란", "빨간"))
#방법2
print("나는 {}살 입니다".format(20))
print("나는 {}색과 {}색을 좋아해요".format("파란","빨간"))
print("나는 {0}색과 {1}색을 좋아해요".format("파란","빨간"))
print("나는 {1}색과 {0}색을 좋아해요".format("파란","빨간"))
#방법3
print("나는 {age} 살이며, {color}색을 좋아해요".format(age=20, color="빨간"))
print("나는 {age} 살이며, {color}색을 좋아해요".format(color="빨간",age=20))
#방법4
#f붙이기
age=20
color="빨간"
print(f"나는 {age} 살이며, {color}색을 좋아해요")
