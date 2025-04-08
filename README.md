# loopDependente
```java
int oP, cN, cS, sN;
        Scanner ler = new Scanner(System.in);

        nC = 0; //declarar como zero pois nao foi respondido ainda
        cS = 0; //declarar como zero pois nao foi respondido ainda
        oP = 1; //declarar como 1 para ir na pergunta

        while (oP != 0) { //enquanto for diferente de zero ira repetir o loop da pergunta e quando for zero ira finalizar a soma
            System.out.println("Digite 1.Continuar ou 0.Parar:");
            oP = ler.nextInt();
            if (oP != 0) { //confirmar se e diferente de zero para ir na peegunta
                System.out.println("Voce gosta de tomate? 1-Sim ou 2-Não");
                sN = ler.nextInt();
                if (sN == 1) { //quando fo respondido sim ira guardar esse resultado no cS(contador dos sim)
                    cS++;
                } else { //quando for nao ira guardar o resultado no cS(contador dos não)
                    cN++;
                }
            } else { //se digitar 0 ira manda-lo a mensagem de tchau
                System.out.println("BYE");
            }
        }

        System.out.println("Pessoas que gostam de tomate:" + cS + " não gostam:" + cN);
    }

}
````
