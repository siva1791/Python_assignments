rows1 = int(input("Enter rows for matrix 1: "))
cols1 = int(input("Enter cols for matrix 1: "))

matrix1 = []

for i in range(rows1):
    a = []
    for j in range(cols1):
        a.append(int(input("{}{} -> ".format(i,j))))
    matrix1.append(a)


rows2 = int(input("Enter rows for matrix 2: "))
cols2 = int(input("Enter cols for matrix 2: "))

matrix2 = []
add_result = []

for i in range(rows2):
    a = []
    for j in range(cols2):
        a.append(int(input("{}{} -> ".format(i,j))))
    matrix2.append(a)

for i in range(rows2):
    a = []
    for j in range(cols2):
        a.append(0)
    add_result.append(a)

for i in range(rows1):
    for j in range(cols1):
        add_result[i][j] = matrix1[i][j] + matrix2[i][j]

print("\nMatrix Addition Result: ")
for i in range(rows1):
    print(add_result[i])

mul_result = []
for i in range(rows2):
    a = []
    for j in range(cols2):
        a.append(0)
    mul_result.append(a)

for i in range(rows1):
   for j in range(cols2):
      for k in range(rows2):
         mul_result[i][j] += matrix1[i][k] * matrix2[k][j]

print("\nMatrix Multiplication Result: ")
for i in range(rows1):
    print(mul_result[i])

trans_matrix1 = []
for i in range(rows2):
    a = []
    for j in range(cols2):
        a.append(0)
    trans_matrix1.append(a)

trans_matrix2 = []
for i in range(rows2):
    a = []
    for j in range(cols2):
        a.append(0)
    trans_matrix2.append(a)


for i in range(rows1):
   for j in range(cols1):
       trans_matrix1[j][i] = matrix1[i][j]

for i in range(rows2):
   for j in range(cols2):
       trans_matrix2[j][i] = matrix2[i][j]

print("\nTranspose of Matrix1: ")
for i in range(rows1):
    print(trans_matrix1[i])


print("\nTranspose of Matrix2: ")
for i in range(rows2):
    print(trans_matrix2[i])
