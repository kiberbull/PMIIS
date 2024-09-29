# PMIIS
# Задача №1: Загрузка на github через git bash.

Переход в указанный каталог

<img width="527" alt="image" src="https://github.com/user-attachments/assets/1c807618-060a-4e8a-bf13-8efd7b14dd2e">

Добавление файлов в индекс для отслеживания изменений и проверка

<img width="476" alt="image" src="https://github.com/user-attachments/assets/cd6f2969-2812-4ca3-9adf-22961d763c22">

Запушим в git

<img width="509" alt="image" src="https://github.com/user-attachments/assets/10964a07-b604-430c-b451-9ef7fcb49499">
<img width="489" alt="image" src="https://github.com/user-attachments/assets/b3b69ce3-c2ed-4e12-9798-a0d4ec204184">

Создание тега

<img width="470" alt="image" src="https://github.com/user-attachments/assets/b47623f8-3d95-4a63-b027-74083bb7d093">

# Описание кода Задание №2 Вариант №14
Напишите две функции. Первая функция заполняет массив случайными значениями, вторая функция выводит массив на экран

    import random
    
    def fill_array_with_random_values(size, min_value=0, max_value=100):
        """
        Функция заполняет массив случайными значениями.
        
        :param size: Размер массива
        :param min_value: Минимальное значение случайного числа (включительно)
        :param max_value: Максимальное значение случайного числа (включительно)
        :return: Массив, заполненный случайными значениями
        """
        array = [random.randint(min_value, max_value) for _ in range(size)]
        return array
    
    def print_array(array):
        """
        Функция выводит массив на экран.
        
        :param array: Массив для вывода
        """
        for element in array:
            print(element)
    
    # Пример использования функций
    
    if __name__ == "__main__":
        size = 10  # Размер массива
        min_value = 1  # Минимальное значение случайного числа
        max_value = 50  # Максимальное значение случайного числа
        
        random_array = fill_array_with_random_values(size, min_value, max_value)
        print("Сгенерированный массив случайных значений:")
        print_array(random_array)
