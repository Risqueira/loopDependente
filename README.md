# loopDependente
```java
int Op, Cn, Cs, Sn;
        Scanner ler = new Scanner(System.in);

        Cn = 0; //declarar como zero pois nao foi respondido ainda
        Cs = 0; //declarar como zero pois nao foi respondido ainda
        Op = 1; //declarar como 1 para ir na pergunta

        while (Op != 0) { //enquanto for diferente de zero ira repetir o loop da pergunta e quando for zero ira finalizar a soma
            System.out.println("Digite 1.Continuar ou 0.Parar:");
            Op = ler.nextInt();
            if (Op != 0) { //confirmar se e diferente de zero para ir na peegunta
                System.out.println("Voce gosta de tomate? 1-Sim ou 2-Não");
                Sn = ler.nextInt();
                if (Sn == 1) { //quando fo respondido sim ira guardar esse resultado no Cs(gaveta dos sim)
                    Cs++;
                } else { //quando for nao ira guardar o resultado no Cn(gaveta dos não)
                    Cn++;
                }
            } else { //se digitar 0 ira manda-lo a mensagem de tchau
                System.out.println("BYE");
            }
        }

        System.out.println("Pessoas que gostam de tomate:" + Cs + " não gostam:" + Cn);
    }

}
````
