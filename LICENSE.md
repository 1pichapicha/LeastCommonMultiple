     Scanner scanner = new Scanner(System.in);

        System.out.print("Введите первое число: ");
        int number1 = scanner.nextInt();

        System.out.print("Введите второе число: ");
        int number2 = scanner.nextInt();

        int lcm = calculateLCM(number1, number2);
        System.out.println("Наименьшее общее кратное: " + lcm);
    }
