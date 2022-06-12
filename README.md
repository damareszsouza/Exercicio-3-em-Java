# Exercicio-3-em-Java

# Exercicio do livro Tutorial de Programação em Java e Orientação a Objetos

# O programa a seguir exemplifica chamadas de métodos, para tal define um objeto que serve
# como contador, a implementação representa a contagem no atributo num que é um número inteiro.
# Os métodos são simples: incrementa adiciona um ao contador em qualquer estado e comeca
# inicializa a contagem em zero. Decrementa faz o oposto de incrementa.


//Classe Contador, arquivo Contador.Java
public class Contador {
public int num; //este é o atributo
//numero do contador
public void incrementa() {
 num = num + 1; //acesso ao atributo
 } 
public void decrementa() {
 num = num - 1;
 }
public void comeca(int n)
//comeca a contar
 {
 num = n;
 }
}

//Classe principal, Arquivo Princ.Java

public class Principal {
 public static void main(String args[]) {
 
 Contador umcont; 
 //declaracao de atributo contador
 umcont = new Contador();
 //alocacao
 umcont.comeca(0);
 System.out.println(umcont.num);
 umcont.incrementa();
 System.out.println(umcont.num);
 }
}
