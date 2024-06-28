# emotion recognition in real time

## Структура
- emotion_recognition_model.ipynb - основной файл с препроцессингом данных, обучением и валидацией классификационной модели.
- frontal_camera.ipynb - работа с фронтальной камерой ноутбука, инференс модели.
- resnet_34_7e.pth - веса предобученной модели.
- haarcascade_frontalface_default.xml - детектор лиц, нужен для работы с фронтальной камерой.

## Инструкция по запуску
Запуск файла emotion_recognition_model ведет к обучению модели с нуля, на ГПУ 1 эпоха занимает ~ 6 минут. 
Для инфренса нужно вызвать метод predict у модели класса $EmotionRecognitionModel$.
