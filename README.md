# Sinifi-Gecme-Durumu-

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        int mat, fizik, turkce, kimya, muzik;
        double ortalama;

            Scanner input = new Scanner(System.in);

        System.out.println("Matematik notunuz: " );
        mat = input.nextInt();

        System.out.println("Turkce notunuz: " );
        turkce = input.nextInt();

        System.out.println("Fizik notunuz: " );
        fizik = input.nextInt();

        System.out.println("Kimya notunuz: " );
        kimya = input.nextInt();

        System.out.println("Muzik notunuz: " );
        muzik = input.nextInt();

        if ((mat<0||mat>100)||(fizik<0||fizik>100) ||(kimya<0||kimya>100)||(turkce<0||turkce>100)
                ||(muzik<0||muzik>100)){
            System.out.println("Geçersiz not girişi yaptınız!!");

        }else {

            ortalama = (mat + fizik + kimya + turkce + muzik) / 5;
            System.out.println("Ortalamanız: " + ortalama);

            if (ortalama > 55) {
                System.out.println("Tebrikler!! Geçtiniz!!");
            } else {
                System.out.println("Maalesef!! Kaldınız!!");
            }
        }
    }
}
