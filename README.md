# Análise de Qualidade do Ar — Ozônio (O3) - 2025

Projeto de análise de qualidade do ar (ozônio, parâmetro 44201) referente a 2025.

Descrição
- Este repositório contém um Jupyter Notebook que realiza limpeza de dados, análise estatística
	e visualizações do AQI (Air Quality Index) para a cidade com mais registros no conjunto de dados.

Conteúdo
- `analise_qualidade_ar.ipynb`: notebook principal com todo o fluxo analítico.
- `daily_44201_2025.csv`: arquivo de dados diário (EPA AQS) usado na análise.
- `analise_qualidade_ar.html`: versão exportada em HTML do notebook (gerada localmente).

Requisitos
- Python 3.8+ (recomendado)
- Pacotes Python: `pandas`, `matplotlib`, `seaborn`, `jupyter` (ou `notebook`), `nbconvert`.

Instalação e execução (exemplo PowerShell)
1. Criar/ativar virtualenv:
```powershell
python -m venv .venv
& .\.venv\Scripts\Activate.ps1
```
2. Instalar dependências:
```powershell
pip install pandas matplotlib seaborn jupyter nbconvert
```
3. Executar o notebook:
```powershell
jupyter notebook analise_qualidade_ar.ipynb
```

Exportar para HTML/PDF
- Para gerar HTML (contendo as saídas executadas):
```powershell
jupyter nbconvert "analise_qualidade_ar.ipynb" --to html --output "analise_qualidade_ar.html"
```
- Gerar PDF via `nbconvert --to webpdf` pode requerer dependências adicionais (Playwright/greenlet). Como alternativa, abra o HTML no navegador e use "Imprimir → Salvar como PDF".

Dados
- Fonte: EPA AQS — https://aqs.epa.gov/aqsweb/airdata/download_files.html
- O arquivo `daily_44201_2025.csv` foi usado diretamente na análise e não é gerado pelo notebook.

Boas práticas Git
- Ignore a virtualenv local adicionando `/.venv/` ao `.gitignore` (já presente neste repositório).

Contato
- Autor: Leonardo da Rocha Lucena

Licença
- Este repositório é para fins acadêmicos. Use conforme as permissões do autor.
