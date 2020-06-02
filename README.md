# Введение в 3D machine learning
![](https://miro.medium.com/max/1400/1*dz0fqQ1KBqIYGexQ_I4SpA.jpeg)
## Содержание
В репозитории содержится код с примерами и данные для серии заметок по 3D ML на [хабр](https://habr.com/ru/users/itmai/posts/).

1)  
   * В ноутбуке `3dml_habr_phygitalism_part_1.ipynb` содержатся примеры коды для [части 1](https://habr.com/ru/company/itmai/blog/503358/).

   * В ноутбуке `raymarch_sdf.ipynb` содержится двумерный пример визуализации объектов, описываемых SDF функциями из [части 1](https://habr.com/ru/company/itmai/blog/503358/).

   * Необходимая для работы с кодом модель `bunny.obj` содержится в папке `data`. 

2) 
   * В ноутбуке `3dml_habr_phygitalism_part_2.ipynb` содержатся примеры коды для [части 2](https://habr.com/ru/company/itmai/blog/504416/).

   * Необходимые для работы с кодом модели `bunny.obj`, `mesh_source.obj`,  `mesh_target.obj` содержатся в папке `data`.
___
## Работа с кодом

### Local

Локальная работа с кодом расчитана на ОС семейства Linux. C PyTorch 3D есть проблемы при работе в Windows.

Для того, чтобы работать с кодом локально, прилагается файл `requirements.txt` со всеми необходимыми зависимостями.

Для запуска jupyter notebook для второй заметки, рекомендуется создать виртуальное окружение с помощью `conda` и установить зависимости из файла `anaconda-env.yaml`.

    conda env create -n имя_окружения_если_оно_не_указано --file .\anaconda-env.yaml

Рекомендуемая версия Python 3.6+

Для установки достаточно выполнить команду:
```
pip install -r requirements.txt
```

При локальной работе с ноутбуками `3dml_habr_phygitalism_part_#.ipynb` не стоит выполнять первую ячейку с установкой зависимостей, если вы уже установили их с помощью `requirements.txt`.

### Colab

Для работы с кодом без локальной установки библиотек, можно запустить jupyter notebook `3dml_habr_phygitalism.ipynb` с помощью [Google colab](https://colab.research.google.com/).

Примеры различных полигональных моделей находятся в директории `data`.

При работе с ноутбуком `3dml_habr_phygitalism_part_2.ipynb` в colab, необходимо дополнительно загрузить модели `mesh_source.obj`,  `mesh_target.obj` из папки `data`.
___
## Источники
Дополнительно прочитать документацию основных рассмотренных фреймворков для работы с 3D данными можно прочитать на домашних страницах проектов:
- [pytorch3d](https://github.com/facebookresearch/pytorch3d)
- [trimesh](https://github.com/mikedh/trimesh) 
  
Больше интересных материалов по работе с 3D, сканированию и технологиям XR можно найти в нашем блоге на [Medium](https://medium.com/phygitalism).
