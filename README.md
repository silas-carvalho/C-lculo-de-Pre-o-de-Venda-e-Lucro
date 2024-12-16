# Cálculo de Preço de Venda e Lucro v1

O projeto "Cálculo de Preço de Venda e Lucro v1" está em desenvolvimento e visa oferecer uma ferramenta robusta e intuitiva para empreendedores. Com ele, será possível calcular preços de venda, lucros e margens de forma precisa, levando em consideração uma variedade de fatores cruciais para a viabilidade e rentabilidade dos negócios.

## Pré-requisitos

Certifique-se de que você tem o Python 3.x instalado em seu sistema. O Python 3.x pode ser encontrado na Microsoft Store.

## Instalar dependências

Windows Power Shell
```bash
pip install colorama
```

Linux ou MacOs
```bash
sudo pip install colorama
```

# Fórmulas

Fórmula de margem escolhida para utilizar na programação
```bash
PV = custo / (1 - (margem + comissão))
```

Parte do código onde a fórmula de margem escolhida foi aplicada
```bash
if margem_lucro >= 1:
    print(f"{Fore.RED}Erro: A margem de lucro deve ser menor que 100% (até 99,99%). A fórmula PV = custo / (1 - margem) resulta em divisão por zero quando a margem é 100% ou mais. Por favor, insira um valor menor.")
    continue

pv = round_decimal(total_com_extras / (1 - (margem_lucro + comissao_vendedor)))
```
