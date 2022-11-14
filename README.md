# Üçgenin alanını hesaplayan program

import java.util.Scanner;

public class ucgenalan {

    public static void main(String[] args){
    
        Scanner giris= new Scanner(System.in);
        
        System.out.println("1. kenarı girin: ");
        double k1=giris.nextInt();
        
        System.out.println("2. kenarı girin: ");
        double k2=giris.nextInt();
        
        System.out.println("3. kenarı girin: ");
        double k3=giris.nextInt();

        double cevre=k1+k2+k3;
        double islem= cevre * (cevre-k1) *  (cevre-k2) * (cevre-k3);
        double alan=Math.sqrt(islem);

        System.out.println("üçgenin çevresi: " +cevre);
        System.out.println("üçgenin alanı: " + alan);

    }
}
