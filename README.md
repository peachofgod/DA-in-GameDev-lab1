# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #1 выполнил(а):
- Бикмухаметова Алина Рафаиловна
- РИ300016
Отметка о выполнении заданий (заполняется студентом):

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * |  |
| Задание 2 | # |  |
| Задание 3 | # |  |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

## Цель работы
Установить Unity, GitHub, VS Code, создать первый проект на Unity и добавить его в Git. 

## Задание 1
Установить Unity и создать первый проект.

![image](https://user-images.githubusercontent.com/76123476/191676858-11c74d65-6e08-422a-ab3e-81398b944470.png)

Добавить его в GitHub.

![image](https://user-images.githubusercontent.com/76123476/191677101-3bfead1a-3577-4439-b4d5-eb1317a1199e.png)

Ссылка на репозиторий: https://github.com/peachofgod/unity

## Задание 2
Создать первую сцену с кубом и шаром, где куб меняет цвет при столкновении с шаром и на консоле выводится текст с кем произошло столкновение.
Код для реализации данной механики:
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class CheckCollider : MonoBehaviour
{
// Start is called before the first frame update
void Start()
{

}

// Update is called once per frame
void Update()
{

}
private void OnTriggerEnter(Collider other) {
Debug.Log("Произошло столкновение с " + other.gameObject.name);
other.GetComponent<Renderer>().material.SetColor("_Color", Color.green);
}
private void OnTriggerExit(Collider other) {
Debug.Log("Завершено столкновение с " + other.gameObject.name);
other.GetComponent<Renderer>().material.SetColor("_Color", Color.red);
}
}
![image](https://user-images.githubusercontent.com/76123476/191678052-cfb82253-a447-4c72-81ae-b613adfa3013.png)
Скриншоты реализации:
![image](https://user-images.githubusercontent.com/76123476/191678225-08841bc1-deda-4f4f-9122-a911026e4bf9.png)
![image](https://user-images.githubusercontent.com/76123476/191678284-b247c5be-305c-4e6a-9963-6e57e920a80d.png)


## Задание 3

## Выводы

Абзац умных слов о том, что было сделано и что было узнано.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |
