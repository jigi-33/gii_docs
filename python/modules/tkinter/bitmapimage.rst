BitmapImage - двухцветное изображение
=====================================

.. py:class:: BitmapImage(name=None, cnf={}, master=None, **kw)

    Наследник :py:class:`Image`

    * `background`, `foreground` - цвета фона и переднего плана для изображения.
    * `file`, `maskfile` - пути к файлу с изображением и к маске (изображению, указывающему какие пиксели будут прозрачными).
    * `data`, `maskdata` - вместо пути к файлу можно указать уже загруженные в память данные изображения.