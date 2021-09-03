<h1 align="center">Shipping Estimation</h1>

<div align="center">
  <img src="./logo.png">
</div>
  
<hr>

Adiciona o botão de calcular frete ao carrinho.

<hr>

<p align="center">
  <a href="#dart-compatibilidade">Compatibilidade & Requisitos</a> &#xa0; | &#xa0; 
  <a href="#checkered_flag-instalação">Instalação, Desinstalação e Reinstalação</a>
</p>

<br>

## :dart: Compatibilidade ##
- [x] Magento 2.4.x & PHP 7.4 
- [x] Magento 2.3.3 & PHP 7.3

## :checkered_flag: Instalação ##

### Instalando
1. Baixe o arquivo .zip deste repositório
2. Crie as pastas `app/code/Tezus/Tezus_ShippingEstimation` e extraia o .zip para essa pasta.
3. Habilite o módulo: `bin/magento module:enable Tezus_ShippingEstimation`
4. Execute os seguintes comandos 
```bash
bin/mangento setup:upgrade && 
bin/magneto setup:di:compile && 
bin/magento setup:static-content:deploy -f && 
bin/magneto c:c && bin/magento c:f
```

### Desinstalando
1. Desabilite o módulo: `bin/magento module:disable Tezus_ShippingEstimation`
2. Remova os arquivos e a pasta `app/code/Tezus/Tezus_ShippingEstimation`;
3. Deletar o registro antigo na tabela `setup_module`
`delete from setup_module where module = 'Tezus_ShippingEstimation'`
4. Execute os seguintes comandos 
```bash
bin/mangento setup:upgrade && 
bin/magneto setup:di:compile && 
bin/magento setup:static-content:deploy -f && 
bin/magneto c:c && bin/magento c:f
```

### Reinstalando
1. Deletar o registro antigo na tabela `setup_module`
`delete from setup_module where module = 'Tezus_ShippingEstimation'`
2. Caso necessário, remova a pasta do módulo `rm -rf app/code/Tezus/Tezus_ShippingEstimation`
3. Baixe o arquivo .zip deste repositório
4. Crie as pastas `app/code/Tezus/Tezus_ShippingEstimation` e extraia o .zip para essa pasta.
5. Habilite o módulo: `bin/magento module:enable Tezus_ShippingEstimation`
6. Execute os seguintes comandos 
```bash
bin/mangento setup:upgrade && 
bin/magneto setup:di:compile && 
bin/magento setup:static-content:deploy -f && 
bin/magneto c:c && bin/magento c:f
```
