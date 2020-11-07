# rockpaper
import java.util.Scanner;
import java.util.Random;

public class rockpaperScissor
{
    public static void main(String[] args)
    {
    Scanner ks=new Scanner(System.in);
    int u=0,pc=0;
        System.out.println("(1)rock \t (2)paper \t (3)scissor");
        u=ks.nextInt();
        Random ran=new Random();
        pc= ran.nextInt(3)+1;
        System.out.println("u chose"+u);
        System.out.println("pc chose"+pc);
        switch (u)
        {
            case 1:
                System.out.println("u chose rock");
            break;
            case 2:
                System.out.println("u chose paper");
            break;
            case 3:
                System.out.println("u chose scissor");
            break;
            default:
                System.out.println("wrong choice");
        }
        switch (pc)
        {
            case 1:
                System.out.println("comp chose rock");
                break;
            case 2:
                System.out.println("comp chose paper");
                break;
            case 3:
                System.out.println("comp chose scissor");
                break;
        }
        if (pc==u)
            {
                System.out.println("its a tie");
            }
        if (pc==1 && u==2)//rock and paper
            {
                System.out.println("u win");
            }
        else if(pc==2 && u==3)//paper and scissor
            {
                System.out.println("u won");
            }
        else if(pc==3&& u==1)//scissor and rock
            {
                System.out.println("u won");
            }
        else if(pc==2&& u==1)//paper and rock
        {
            System.out.println("com wons");
        }
        else if(pc==3&& u==2)//scissor and paper
        {
            System.out.println("comp won");
        }
        else if(pc==1&& u==3)//rock and scissor
        {
            System.out.println("u won");
        }
    }
}
