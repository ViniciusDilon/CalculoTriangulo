import java.util.Scanner;

class CalculoTriangulo {
  
	public static void main(String args[]){  
   
    		Scanner teclado = new Scanner(System.in);
    
    		double x;
			double y;
			double z;
			double area;
			double p;
			double conversao;
			
			System.out.printf("Digite o valor do lado x: \n"); 
				x = teclado.nextDouble();
			
			System.out.printf("Digite o valor do lado y: \n"); 
				y = teclado.nextDouble();
				
			System.out.printf("Digite o valor do lado z: \n"); 
				z = teclado.nextDouble();
			
				System.out.printf("-------------------------------------------\n\n");
			
			if(x == y && x == z){
				System.out.printf("O triangulo e do tipo equilatero! \n\n");
				System.out.printf("-------------------------------------------\n\n");
			}
			
			if(x != y && x != z){
				System.out.printf("O triangulo e do tipo escaleno! \n\n");
				System.out.printf("-------------------------------------------\n\n");
			}
			
			if((x == y && x != z) || (x != y && x == z)){
				System.out.printf("O triangulo e do tipo isosceles! \n\n");
				System.out.printf("-------------------------------------------\n\n");
			}
			
			p = (x + y + z) / 2;
				System.out.printf("O valor do perimetro e: " + p + "cm \n\n");
				
				System.out.printf("-------------------------------------------\n\n");
			
			area = Math.sqrt(p * (p - x) * (p - y) * (p - z));
				System.out.printf("O valor da area e: " + area + "cm \n\n");
				
				System.out.printf("-------------------------------------------\n\n");
				
			conversao = area / 100;
				System.out.printf("O valor da area em metros e: " + conversao + "m \n\n");
			
    		System.exit(0);
	}

}
