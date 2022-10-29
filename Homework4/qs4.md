1) В случае, когда в нескольких классах есть одни и те же методы, создают родительский класс, в который входят все эти методы. Тогда эти несколько классов являются дочерними от родительского, и они автоматически обладают всеми методами из родительского класса, а неповторяющиеся методы прописываются отдельно в каждом из классов.

2) super.method() вызывает родительский метод в дочернем классе. Тогда поиск вызываемого метода будет осуществляться в ширину, в случае, когда родитель не единственный (то есть, поиск начнется с конца и пойдет по старшинству родителей).

3) Обработка исключений нужна, чтобы програма решала проблемы связанные с ошибками, которые совершает пользователь, чтобы программа не зависала. При обработки исключения программа выдаёт ошибку с указанием на исправление или продолжает работу. Но это замедляет работу программы, поэтому использование обработки исключений, где мы не можем ожидать ошибки, некорректно.

4) Можно создать свой класс исключений, который должен быть наследуемым от класса Exception. Тогда это новое исключение может быть вызванно с помощью raise. 