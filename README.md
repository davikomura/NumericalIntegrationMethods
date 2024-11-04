# Numerical Integration Methods

### Descrição
Este projeto implementa cinco métodos de integração numérica em Python utilizando a biblioteca NumPy. Esses métodos são úteis para calcular aproximações de integrais definidas quando uma solução analítica não é prática ou possível. Abaixo estão os métodos implementados:

- **Regra do Trapézio**
- **Regra de Simpson**
- **Quadratura de Gauss**
- **Método de Monte Carlo para Integração**
- **Método de Romberg**

### Pré-requisitos
- Python 3.x
- NumPy

### Instalação
Clone o repositório e instale os pacotes necessários:

```bash
git clone https://github.com/username/NumericalIntegrationMethods.git
cd NumericalIntegrationMethods
pip install -r requirements.txt
```

### Uso
Exemplos de uso de cada método estão disponíveis no arquivo `examples/example_usage.py`. Cada método está implementado em um arquivo separado dentro da pasta `integration_methods/`. Aqui estão exemplos de como usar cada método:

#### Exemplo de Uso - Regra do Trapézio
```python
from integration_methods.trapezoidal import trapezoidal_rule

# Função para integrar
def f(x):
    return x**2

# Intervalo e número de subdivisões
a, b = 0, 1
n = 100

# Calcular a integral aproximada
resultado = trapezoidal_rule(f, a, b, n)
print(f"Resultado da integração pela Regra do Trapézio: {resultado}")
```

#### Outros Métodos
Exemplos semelhantes estão disponíveis para:
- `simpson.py` - Regra de Simpson
- `gauss_quadrature.py` - Quadratura de Gauss
- `monte_carlo.py` - Método de Monte Carlo
- `romberg.py` - Método de Romberg

### Testes
Os testes unitários estão localizados na pasta `tests/`. Para rodar os testes, utilize o `pytest`:

```bash
pytest
```

### Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.

### Licença
Este projeto está licenciado sob a [MIT License](LICENSE).
