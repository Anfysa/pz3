Практическое задание 3
Поиск центра лазерного пятна состояил из следующих этапов:
1. С помощью функции cv2.cvtColor преобразовали изображение в оттенки серого, потом с помощью функции cv2.threshold преобразовали изображение в черно-белое
2. С помощью функции cv2.findContours нашли контур лазерных точек
3. В цикле находим наибольшую площадь из найденных контуров (те это и есть наша лазерная точка)
4. Находим прямоугольник, ограничивающий эту площадь, и в нем вычисляем центр - это центр лазерной точки
