import numpy as np

# Пример матрицы размерности n * m
n, m = 4, 5  # Размерности матрицы
matrix = np.random.rand(n, m)  # Генерация случайной матрицы
print("Исходная матрица:")
print(matrix)

# Номер столбца для удаления (k)
k = 2  # Удаляем третий столбец (индексация с 0)

# Удаление k-го столбца
if 0 <= k < m:
    modified_matrix = np.delete(matrix, k, axis=1)
    print("\nМатрица после удаления столбца:")
    print(modified_matrix)
else:
    print("Ошибка: индекс столбца выходит за пределы матрицы.")
