# KATA Academy. PRE-PROJECT

## Поток:
### Группа: 
### Студент: 
___

# Практическая задача 2.1.4 Java pre-project. Практическая задача 2.1.3. Spring Beans.

---
## Практическая задача

### Условие:
Склонируйте заготовку проекта по [ссылке](https://github.com/KataAcademy/PP_2_1_3_SpringBeans).

Поработаем со связыванием бинов.  
Вызывать бины из контекста хорошо, но не так удобно, как связывать их автоматически.  
Для работы аннотаций связывания, я добавил в Maven ядро Спринга,
так мы имеем совершенно рабочее Spring-приложение, пусть и без дополнительных модулей.  
В компоненте **AnimalCage** есть поле типа **Animal**,
которое связано с помощью аннотации **@Autowired**. При выполнении программы
DI-контейнер подтянет сюда бин, подходящий по типу.

### Задание:

1) Создайте бин **Dog**, унаследуйте его от **Animal**. Создайте на основе этого класса компонент.
2) Запустите приложение и проверьте, что было выброшено исключение
   **NoUniqueBeanDefinitionException**. Это произошло из-за того,
   что существует 2 бина с типом **Animal**.
3) Прочитайте о связывании бинов по имени и свяжите **AnimalCage** c бином **Dog**
   через абстрактный класс **Animal**.
4) На основе класса **Timer** создайте бин. Свяжите с **AnimalCage**.
   Проверьте, что при выполнении метода main время, которое пишет таймер, одно и тоже.
5) Раскомментировать тест из заготовки и проверить своё решение.