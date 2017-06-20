# Sintaxe

Toda instrução declarada no php deve ser terminada com o **ponto e vírgula**/**semi-colon** (;) , exemplo:

````php
<?php
    echo "Hello World";
    1 + 1;
    array_sum(array(1,2,3,4,5,6,7,8,9));
    ...
?>    
````    

## Tags

Nessa parte o manual ( PHP.net ) é muito claro, vejamos:

> "Quando o PHP interpreta um arquivo ele procura pelas tags de abertura e fechamento, \<?php e ?\>, que dizem ao PHP 
> para iniciar ou parar a interpretação do código entre elas. A interpretação dessa maneira, permite o PHP ser incluído em vários tipos de documentos, pois tudo que está fora dessas tags é ignorado pelo interpretador do PHP."

exemplo de abertura e fechamento das tags:

````php
<?php 
# abrimos
# ... nosso código ...
# fechamos
?> 
````
ou
 
````php
<?= $foobar; ?> // imprime o variável $foobar
````

````php
<?
# O PHP também permite a tag curta <? (cujo uso é desencorajado pois essa opção está disponível somente quando
# habilitada na diretiva short_open_tag no arquivo de configuração php.ini, ou quando o PHP tiver sido compilado com a
# opção --enable-short-tags ).
?> 
````

## Comentários

O PHP suporta comentários no estilo 'C', 'C++' e do Unix shell (estilo Perl), exemplo:

````
<?php

// USADO PARA UMA LINHA DE COMENTÁRIO ÚNICO
// DEVE SER REPETIDO PARA LINHAS MÚLTIPLAS ...

# OUTRA OPÇÃO 
# LINHA
# POR
# LINHA

/* USADO PARA BLOCOS DE CÓDIGO. */

/**
 * Usado PARA BLOCOS DE COMENTÁRIOS MAIS DETALHADOS.
 */


````

## ChangeLog

|Versão	|Descrição                                                                                  |
|-------|-------------------------------------------------------------------------------------------|
|7.0.0  |As tags ASP <%, %>, <%= e a script tag \<script language="php"\> foram removidos do PHP.   |
|5.4.0  |A tag <?= sempre está disponível, independente do da configuração short_open_tag ini.      |