# emotion recognition in real time

## Постановка задачи
Перед премьерой фильмов/сериалов аудитории обычно показывают трейлеры - короткие ролики, состоящие из наиболее зрелищных моментов. Для составления трейлеров некоторой контрольной группе показывают фильм, а эксперты в это время анализируют их эмоции, тем самым получая возможность найти нужные для трейлера моменты. Однако обрабатывать результаты вручную неэффективно, поэтому требуется приспособить нейросеть для классификации эмоций, а также снабдить ее возможностью работать в реальном времени.

## Решение (дописать)
### Структура
- emotion_recognition_model.ipynb - сверточная сеть для классификации.
- frontal_camera.ipynb - работа с фронтальной камерой ноутбука, инференс модели.
- resnet_34_7e.pth - веса предобученной модели.
- haarcascade_frontalface_default.xml - детектор лиц, нужен для работы с фронтальной камерой.
### Сверточная нейросеть
ResNet-34 и MLP-надстройка для классификации, параметры обучения
### Работа в реальном времени
Детектро лиц + фронтальная камера, работает только на локале.

## Результаты
Время обучения и инференса, метрики

## Инструкция по запуску
Запуск файла emotion_recognition_model ведет к обучению модели с нуля, на GPU 1 эпоха занимает ~ 6 минут. 
Для инфренса нужно вызвать метод predict у модели класса $EmotionRecognitionModel$.
