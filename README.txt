Специальность: 09.02.07 Информационные системы и программирование
Квалификация: Тестировщик

ОТЧЕТ
РАЗРАБОТКА МОБИЛЬНЫХ ПРИЛОЖЕНИЙ
Практическая работа №1

Выполнил студент
Группы Т50-1-22
А. О. Константинов
«____» _________ 2023 года

Проверил преподаватель
___________Д. А. Пахомов
«____» _______2023 года

Цель работы:
Создать программу обладающую следующим функционалом: 
1.приветствие с пользователем 
2.Ввод персональных данных(2 персональных данных) 
3. Проверка на совершеннолетие (18 лет). 
4.  Нахождение периметра, площади, радиуса
Ход работы: 
1.	Создание меню выбора между двух программ 

            System.out.println("Здравствуй, пользователь!");
            System.out.println("Выберите программу: \n 1.Ввод перс. данных, проверка на возраст \n 2.Нахождение периметра, площади, радиуса ");
            Scanner o = new Scanner(System.in);
            System.out.print("Введи число: ");
            int n = o.nextInt();


2.	Создание условных кострукций для функционирования меню выбора

 if (n == 1) {
                Scanner f = new Scanner(System.in);
                System.out.print("Введите ваше имя: ");
                String t = f.nextLine();
                System.out.println("Приветствуем, " + t);
                System.out.print("Введите ваш номер телефона: ");
                String s = f.nextLine();
                System.out.println("Ваш номер - " + s);
                System.out.print("Введите ваш Возраст: ");
                int x = f.nextInt();
                if (x < 18) {
                    System.out.print("К сожалению, Вы ещё не совершеннолетний, вам - " + x);
                } else if (x >= 18) {
                    System.out.print("Поздравляем! Вы совершеннолетний, вам - " + x);
                }


            } else if (n == 2) {
                System.out.print("\nЧто вы хотите найти? \n1.Периметр \n2.Площадь \n3.Радиус ");
                Scanner f = new Scanner(System.in);
                int t = f.nextInt();

3.	Создание условных конструкций для программы по нахождению периметра, площади и радиуса

if (t == 1) {
                    System.out.print("Периметр какой фигуры вы хотите найти? \n1.Четырехугольник \n2.Треугольник");
                    Scanner e = new Scanner(System.in);
                    int d = e.nextInt();
                    if (d == 1) {
                        System.out.print("Введите длину 4-х сторон \n");
                        Scanner v = new Scanner(System.in);
                        int k = v.nextInt();
                        int z = v.nextInt();
                        int x = v.nextInt();
                        int b = v.nextInt();
                        int a = k + z + x + b;
                        System.out.print("Периметр четырехугольника равен: " + a);
              } else if (d == 2) {
                        System.out.print("Введите длину 3-х сторон \n");
                        Scanner v = new Scanner(System.in);
                        int k = v.nextInt();
                        int z = v.nextInt();
                        int x = v.nextInt();

                        int a = k + z + x;
                        System.out.print("Периметр треугольника равен: " + a);
               }
               } else if (t == 2) {
                    System.out.print("Введите длину двух сторон четырехугольника \n");
                    Scanner g = new Scanner(System.in);
                    int k = g.nextInt();
                    int z = g.nextInt();


                    int a = k * z;
                    System.out.print("Площадь четырехугольника равна: " + a);
               } else if (t == 3) {
                    System.out.print("Введите длину круга \n");
                    Scanner g = new Scanner(System.in);
                    int k = g.nextInt();
                    double a = k / (2 * 3.14);
                    System.out.print("Радиус круга равен: " + a);
               }

Вывод: Была создана программа обладающая следующим функционалом: 
1.приветствие с пользователем 
2.Ввод персональных данных(2 персональных данных) 
3. Проверка на совершеннолетие (18 лет). 
4.  Нахождение периметра, площади, радиуса
