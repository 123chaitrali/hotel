# hotel
package multithreading;

/**
 *
 * @author ADMIN
 */
 

public class Hotel{
    public static void main(String[] args) {
        Hotel1 t1 = new Hotel1();
        Hotel2 t2 = new Hotel2();
        Hotel3 t3 = new Hotel3();

        t1.start();
        t2.start();
        t3.start();
    }

    static class Hotel1 extends Thread {
        @Override
        public void run() {
            int i = 0;
            while (i < 2) {
                System.out.println("Serve burger first table");
                System.out.println("One table");
                i++;
            }
        }
    }

    static class Hotel2 extends Thread {
        @Override
        public void run() {
            int i = 0;
            while (i < 2) {
                System.out.println("Serve fries second table");
                System.out.println("Second table");
                i++;
            }
        }
    }

    static class Hotel3 extends Thread {
        @Override
        public void run() {
            int i = 0;
            while (i < 2) {
                System.out.println("Serve pepsi third table");
                System.out.println("Third table")
                i++;
            }
        }
    }
}

        
       
    
    
    
    
    
