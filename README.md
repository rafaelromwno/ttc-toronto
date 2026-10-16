# Atrasos do metrô de Toronto (TTC)

Projeto acadêmico de Data Mining sobre o [TTC Subway Delay Data](https://open.toronto.ca/). O notebook segue a metodologia KDD: seleção, limpeza, transformação, mineração e interpretação.

Perguntas cobertas: principais causas, padrões por dia e hora, linhas e estações mais críticas, e impacto em minutos de atraso e intervalo entre trens.

## Como rodar

```bash
python3 -m venv .venv
.venv/bin/pip install -r requirements.txt
.venv/bin/jupyter lab src/ttc_subway_delay_kdd.ipynb
```

O notebook procura `TTC Subway Delay Data since 2025.csv` em `src/`.

## Dados

| Coluna | Conteúdo |
|---|---|
| `Date`, `Time`, `Day` | Quando o incidente ocorreu |
| `Station`, `Line`, `Bound`, `Vehicle` | Onde e em qual trem |
| `Code` | Código TTC da causa |
| `Min Delay`, `Min Gap` | Minutos de atraso e intervalo até o próximo trem |
