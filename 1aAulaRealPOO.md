# No Gradle:

## em "App.java":

```
package ads.poo;

public class App {
    public static void main(String[] args) {

    Caneta bic = new Caneta();

    System.out.println(bic.isAberta());

    bic.abrirFechar();

    bic.definirCor("branco");

    System.out.println(bic.isAberta());
    System.out.println(bic.getCor());

    }
}
```

---------------------------------------
## em "Caneta.java":

```
package ads.poo;

public class Caneta {

    // atributos
    private String cor;
    private double nivelTinta;
    private boolean aberta;

    public void definirCor(String c){
        cor = c;
    }

    public String getCor(){
        return cor;
    }

    public void definirNivelTinta(double n){
        nivelTinta = n;
    }

    public void abrirFechar(){
        aberta = !aberta;

    }

    public boolean isAberta(){
        return aberta;
    }
}
```