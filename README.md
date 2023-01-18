# 8.3-Gitlab

### Задание 1

![image](https://user-images.githubusercontent.com/121398221/213275655-93b685f9-9b3f-43af-9359-ad15ae5b8e70.png)
![image](https://user-images.githubusercontent.com/121398221/213275748-11ffb26c-c693-4098-a81a-f9dd6729119f.png)

---

### Задание 2

В ПРОЦЕССЕ
Всё делал по инструкции, но почему-то Pipeline застрял:
![image](https://user-images.githubusercontent.com/121398221/213276624-a99c08ce-5cc7-4007-b34e-a2f8ad0ef81a.png)

Использовал из лекции:

stages:
  - test
  - build

test:
  stage: test
  image: golang:1.17
  script: 
   - go test .

build:
  stage: build
  image: docker:latest
  script:
   - docker build .


---
