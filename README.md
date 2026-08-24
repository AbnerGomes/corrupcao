# Ficha Corrida

Site estático (uma única página, sem build, sem dependências) com uma linha do
tempo ano a ano (2005–2026) das investigações, denúncias e condenações por
corrupção envolvendo três nomes cotados para a disputa presidencial de 2026:

- Luiz Inácio Lula da Silva
- Renan Calheiros
- Flávio Bolsonaro

## Como rodar localmente

Não precisa de build nem de servidor: basta abrir `index.html` no navegador,
ou servir a pasta com qualquer servidor estático, por exemplo:

```bash
python3 -m http.server 8000
# depois abra http://localhost:8000
```

## Como está organizado

- `index.html` — a página inteira (HTML + CSS + JS embutidos, sem dependências
  externas além das fontes do Google Fonts).

## Metodologia (resumo)

Cada célula do "livro-razão" ano × candidato é colorida pelo estágio mais
grave alcançado naquele ano:

- **Verde** — nenhuma investigação, acusação ou condenação por corrupção
  documentada para aquele nome, naquele ano.
- **Laranja** — investigação, denúncia formal, indiciamento ou julgamento sem
  condenação (inclusive absolvições e arquivamentos).
- **Vermelho** — condenação formal em algum grau de jurisdição naquele ano,
  mesmo que revista ou anulada depois (a anulação é sempre indicada no texto
  da célula e no ano em que ocorreu).

Investigações contra terceiros (familiares, assessores, aliados) só entram na
ficha do próprio candidato quando ele é formalmente investigado, denunciado
ou condenado — não pela proximidade com o investigado.

Todas as fontes usadas estão listadas ao final da própria página, agrupadas
por candidato. Nenhuma delas é a Wikipédia: priorizamos portais oficiais
(STF, Agência Brasil) e veículos de imprensa com apuração própria (ConJur,
CNN Brasil, ISTOÉ, Exame, JOTA, CartaCapital, Correio Braziliense, Gazeta do
Povo, Brasil de Fato, entre outros).

## Aviso

Este conteúdo é informativo, compilado a partir de reportagem pública e
decisões judiciais, e **não é aconselhamento jurídico nem eleitoral**. A
situação de qualquer processo pode mudar — para o status mais atual, consulte
diretamente [STF](https://portal.stf.jus.br/), [STJ](https://www.stj.jus.br/),
[MPF](https://www.mpf.mp.br/) e [TSE](https://www.tse.jus.br/).

Compilado em 24 de agosto de 2026.
