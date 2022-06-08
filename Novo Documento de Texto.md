# 1 - Sistema de grid Bootstrap
* O sistema grid Bootstrap usa vários containers, linhas e colunas para arranjar e alinhar conteúdo. Ele é feito com flexbox e é, totalmente, responsivo.

* O exemplo abaixo cria três colunas de larguras idênticas em dispositivos pequenos, médios, grandes e extra grandes, usando nossas classes grid pré-definidas. Estas colunas são centralizadas na página, usando o elemento pai __.container__.
```
<div class="container">
  <div class="row">
    <div class="col-sm">
      Uma de três colunas
    </div>
    <div class="col-sm">
      Uma de três colunas
    </div>
    <div class="col-sm">
      Uma de três colunas
    </div>
  </div>
</div>
```

# 2 - Grid empilhado na horizontal

* Grid empilhado na horizontal é um sistema simples de grid que começa no mobile antes de ir para dispositivos como desktop tento uma aparecencia em horizontal não mais na vertical como um dispositivo mobile.
* O exemplo abaixo teremos duas colunas de 50% por 50%
```
<div class="container">
  <div class="row">
    <div class="col-sm-6 bg-success">
      <p>Lorem ipsum...</p>
    </div>
    <div class="col-sm-6 bg-warning">
      <p>Sed ut perspiciatis...</p>
    </div>
  </div>
</div>
```
> __Dica__: você pode transformar qualquer layout de largura fixa em um layout de largura total alterando a .containerclasse para .container-fluid.

* As númerações nas classes de cada elemento significa a quantidade de colunas que a dev deve conter, tendo assim um valor máximo de 12 colunas

## Colunas de layout automático
* Com __Bootstrap 5__ conseguimos ter larguras iguais para qualquer dispositivo seja ele mobile ou desktop, retirando a númeração de cada classe e deixando apenas o nome da classe e os elementos se ajustaram automaticamente como no exemplo abaixo.
```
 <!-- Two columns: 50% width on all screens, except for extra small (100% width) -->
<div class="row">
  <div class="col-sm">1 of 2</div>
  <div class="col-sm">2 of 2</div>
</div>

<!-- Four columns: 25% width on all screens, except for extra small (100% width)-->
<div class="row">
  <div class="col-sm">1 of 4</div>
  <div class="col-sm">2 of 4</div>
  <div class="col-sm">3 of 4</div>
  <div class="col-sm">4 of 4</div>
</div> 
```

# 3 - Grid Extra Pequeno
* Grid para dispositivos mobile com tamnho menor que 576px. Para uma divisão de duas colunas um de 25% por uma de 75% para qualquer dispositivo (extra pequeno, pequeno, médio, grande, xlarge e xxlarge), adicionamos as classes ``` col-3 ``` e ``` col-9 ```, contabilizando 12 colunas.
1. Exemplo:
```
<div class="col-3">....</div>
<div class="col-9">....</div>
```

# 4 - Grade Pequena
* Grid para dispositivos mobile com tamanho igual ou maior que 576px. Para uma divisão de duas colunas um de 25% por uma de 75% para qualquer dispositivo (extra pequeno, pequeno, médio, grande, xlarge e xxlarge), adicionamos as classes ``` col-sm-3 ``` e ``` col-sm-9 ```, contabilizando 12 colunas.
1. Exemplo:
```
<div class="col-sm-3">....</div>
<div class="col-sm-9">....</div>
```

# 5 - Grade média
* Grid para dispositivos como tables ou notebooks com tamanho igual ou maior que 768px. Para uma divisão de duas colunas um de 25% por uma de 75% para qualquer dispositivo (extra pequeno, pequeno, médio, grande, xlarge e xxlarge), adicionamos as classes ``` col-md-3 ``` e ``` col-md-9 ```, contabilizando 12 colunas.
> Mas em dispositivos médios o design pode ser melhor com uma divisão de 50%/50%.
1. Exemplo:
```
<div class="col-sm-3 col-md-6">....</div>
<div class="col-sm-9 col-md-6">....</div>
```
* No tamanho pequeno temos as classes ``` sm ```(small) e no médio ``` md ```.

# 6 - Grade Grande
* Grid para dispositivos como notebooks ou desktop com tamanho igual ou maior que 992px. Para uma divisão de duas colunas um de 25% por uma de 75% para qualquer dispositivo (extra pequeno, pequeno, médio, grande, xlarge e xxlarge), adicionamos as classes ``` col-lg-3 ``` e ``` col-lg-9 ```, contabilizando 12 colunas.
> Mas em dispositivos grandes o design pode ser melhor com uma divisão de 33%/66%.
1. Exemplo:
```
<div class="col-sm-3 col-md-6 col-lg-4">....</div>
<div class="col-sm-9 col-md-6 col-lg-8">....</div>
```
* No tamanho pequeno temos as classes ``` sm ```(small), no médio ``` md ```(medium) e no grande ``` lg ```(large).

# 7 - Grade Extra Grande
* Grid para dispositivos como desktop ou TV's com tamanho igual ou maior que 1200px. Para uma divisão de duas colunas um de 25% por uma de 75% para qualquer dispositivo (extra pequeno, pequeno, médio, grande, xlarge e xxlarge), adicionamos as classes ``` col-xl-3 ``` e ``` col-xl-9 ```, contabilizando 12 colunas.
> Mas em dispositivos xlarge o design pode ser melhor com uma divisão de 20%/80%.
1. Exemplo:
```
<div class="col-sm-3 col-md-6 col-lg-4 col-xl-2">....</div>
<div class="col-sm-9 col-md-6 col-lg-8 col-xl-10">....</div>
```
* No tamanho pequeno temos as classes ``` sm ```(small), no médio ``` md ```(medium), no grande ``` lg ```(large) e no extra grande ``` xl ```(extra large).

# 8 - Grade Extra Extra Grande
* Grid para dispositivos como desktop ou TV's com tamanho igual ou maior que 1400px. Para uma divisão de duas colunas um de 25% por uma de 75% para qualquer dispositivo (extra pequeno, pequeno, médio, grande, xlarge e xxlarge), adicionamos as classes ``` col-xxl-3 ``` e ``` col-xxl-9 ```, contabilizando 12 colunas.
> Em dispositivos pequenos e extra pequenos, ele empilhará automaticamente (100%)
1. Exemplo:
```
 <div class="container-fluid">
  <div class="row">
    <div class="col-md-6 col-xxl-3">
      <p>Lorem ipsum...</p>
    </div>
    <div class="col-md-6 col-xxl-9">
      <p>Sed ut perspiciatis...</p>
    </div>
  </div>
</div> 
```
* Usando o ``` XXL ```(extra extra large), precisamos especificar apenas o ``` col-xxl-6 ``` sem o ``` md ``` nem o ``` sm ```, dispositivos xxlarge dividirão 50% por 50%, dispositivos ``` xl ```, ``` lg ```, ``` md ```, ``` sm ``` E ``` xs ```, ele será empilhado verticalmente (100% de largura).