# Демо версия годовая контрольная работа 2021-2022

1. 101110

1. 3

1. 9

1. 8

1. 0

1. 255,53

1. 173,671875

1. умножение;  Λ;

1. сложение; V;

1. истина и ложь;

1. г) логика.

1. Все ученики, выбравшие английский язык, могут учиться в 9В классе.

1. C2:D11

1. Е$1

1. кошка

1. сентябрь, декабрь, май

1. 46, 80, 75

1. 6432

1. 5

1. 10

1. X[k] := 2*X[k-1]

1. X[k]:=2*k-1

1. X[k]>0

1.

```py
arr = list(map(int, input().split()))

res1, res2 = 0, len(arr) - 1

for i in range(len(arr)):
  if arr[i] > arr[res1]:
    res1 = i

for i in range(len(arr)):
  if arr[i] > arr[res2] and i != res1:
    res2 = i

if arr[res2] > arr[res1]:
  res1, res2 = res2, res1

print('Максимальный элемент: A[{}]={}\nВторой максимум: A[{}]={}'.format(res1, arr[res1], res2, arr[res2]))
```

25.

```py
arr = list(map(int, input().split()))

res = 0
count = 0

for i in range(len(arr)):
  if arr[i] > arr[res]:
    res = i
    count = 0
  if arr[i] == arr[res]:
    count += 1

print('Максимальное значение {}\nКоличество элементов {}'.format(arr[res], count))
```

26.

```py
a = list(map(int, input().split()))

res = -1

for i in range(len(a)):
  if a[i] % 10 == 2 or a[i] * -1 % 10 == 2:
    res = i
    break

if res != -1:
  print('Нашли: A[',res, ']=', a[res], sep='')
else:
  print('Не нашли.')
```
