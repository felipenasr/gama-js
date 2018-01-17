# Gama Academy + Caelum

Curso de JS oferecido pela Caelum em parceria com a Gama Academy. Parte do treinamento da Avanade.



### Funcionalidades do projeto
1 - Apagar o cartão:
```
<button onclick="this.parentNode.parentNode.remove()" class="opcoesDoCartao-remove opcoesDoCartao-opcao" tabindex="0">
```
- this para referenciar o elemento;
- Utilizando nodeParent para remover o cartão.

2 - Implementar botão que vria variação entre Linha e Blocos.

- Códio que altera o texto do botão no clique;
```
function mudaTexto() {
    if(this.textContent == "Blocos"){
        this.textContent = "Linhas";
    }else{
        this.textContent = "Blocos";
        
    }
}
```

- Código que muda o layout dos cartões ao clicar no btn;

```
function mudaLayout(){
    if(mural.classList.contains('mural--linha')){
        mural.classList.remove('mural--linha');
    }else{
        mural.classList.add('mural--linha');
    }
}
```

- Implementa o Event Listiner para execuar as duas funções ao clicar no botão;

```
btn.addEventListener('click', mudaLayout)
btn.addEventListener('click', mudaTexto)
```


### Anotações gerais

