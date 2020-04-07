# ApiCongrega
Esse projeto é de minha autoria para estudos de apis.

###Objetivos:
1. Estudo de estruturas api/rest
2. Produzir uma api simples que retorno o Hinário da Igreja Env. Congregacilnal


### Ajustes em 2020.03.11

1. Correção para emissão de notas com produtos que possuem codigo ANP
> * O critério adotado para o preenchimento dos campos da tag *<comb>* é que seja informado no cadastro do produto o codigo ANP e não mais o tipo da Empresa. [Referencia](https://www.oobj.com.br/bc/article/rejei%C3%A7%C3%A3o-660-cfop-de-combust%C3%ADvel-e-n%C3%A3o-informado-grupo-de-combust%C3%ADvel-como-resolver-274.html)
2. Correções para importação de XML.
> * Adicionado função para retirar espaços em branco da descrição das mercadorias na nota do fornecedor do cliente para evitar erros na geração dos arquivos SPED
> * Reconhecimento de produtos por EAN ajustado para buscar primeiramente por *ItensCodigos* evitando alguns erros de reconhecimento da mercadorias
> * Ajuste para importação de notas de Devoluçao ,*(Finaliade = 4)*), que não tem alguns elementos no XML iguais as notas de Finaliade=1, de Venda.
