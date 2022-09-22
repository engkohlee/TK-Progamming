import com.sun.source.tree.NewArrayTree;

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        Scanner scan = new Scanner(System.in);
        boolean y = true;
        int counter = 0;
        String ulang;


        System.out.println("Masukkan Nama anda [1... 25] : ");
        String input = scan.nextLine();
        System.out.println("Masukkan NIM anda [Harus 10 karakter]");
        int NIM = scan.nextInt();

        System.out.println("@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@");

        System.out.println("Registrasi Sukses!");
        System.out.println("Selamat Datang " + input + " [NIM : " + NIM + " ]");
        System.out.println("Mari belajar bermacam-macam bilangan");

        System.out.println("Masukan Sembarang Angka [5..20]: ");
        int x = scan.nextInt();
        System.out.println("@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@\n");

        System.out.println("Deret Bilangan");
        System.out.println("#######################");
        System.out.println(x + " Bilangan Genap  = ");
        int sementara = 0, total = 0;
        for (int a = 1; a <= x; a++) {
            sementara = a * 2;
            System.out.print(sementara + " ");
            total = total + sementara;
        }
        System.out.println("Total   = " + total + " ");

        total = 0;
        sementara = 0;

        System.out.println(x + "Bilangan Ganjil = ");
        for (int a = 1; a <= x; a++) {
            sementara = (a * 2) - 1;
            System.out.print(sementara + " ");
            total = total + sementara;
        }
        System.out.println("Total   = " + total + " ");

        total = 0;
        sementara = 0;

        System.out.println(x + "Bilangan Fibonacci = ");
        int b = 0, c = 0;
        for (int a = 1; a < -x; a++) {
            sementara = b + c;
            System.out.print(sementara + " ");
            b = c;
            c = sementara;
            total = total + sementara;
            System.out.println("Total   = " + total + " ");

        }

        while (y) {
            System.out.print("Anda mau ulang (y/t) : ");
            ulang = scan.nextLine();

            if (ulang.equalsIgnoreCase("t")) {
                y = false;


            }

        }


    }
}





