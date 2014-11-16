---
title:  "Ваша первая программа"
layout: "chapter"

---

Традиционно, первая программа, с которй начинается изучение любого языка программирования, называется «Hello World» — она просто выводит в терминал строку `Hello World`. Давайте напишем её используя Go.

Сначала создадим новую директорию, в которой будем хранить нашу программу. Установщик, использованный в главе 1 создал в вашей домашней директории каталог `Go`. Создайте директорию, под названием `~/Go/src/golang-book/chapter2` (где `~` означает вашу домашнюю директорию). Из терминала вы можете сделать это, введя следующие команды:

    mkdir Go/src/golang-book
    mkdir Go/src/golang-book/chapter2

Используя ваш текстовый редактор, напишите следующее:

    package main

    import "fmt"

    // this is a comment

    func main() {
        fmt.Println("Hello World")
    }

Убедитесь, что ваш файл идентичен показанному здесь примеру и сохраните его под именем `main.go` в созданной ранее директории. Откройте новое окно терминала и введите следующее:

    cd Go/src/golang-book/chapter2
    go run main.go

В терминале должно появиться сообщение `Hello World`. Команда `go run` берет указанные файлы (разделяемые пробелом), компилирует их в исполняемые файлы, сохраняет во временной директории и запускает. Если вы не увидели `Hello World`, то веронятно, где-то была допущена ошибка. Компилятор даст вам подсказки о том, где она заключается. Как и большинство компиляторов, Go крайне педантичен и не прощает ошибок.