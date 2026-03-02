# senai-techguard-ndvi-semana5

Atividade da Semana 5 do projeto Americas TechGuard (SENAI), com foco em analise de NDVI e discussao tecnica sobre risco de inundacao.

## Objetivo
- Executar o notebook base de NDVI.
- Replicar a analise em nova regiao.
- Gerar mapa, histograma e estatisticas para comparacao.

## Estrutura do projeto
- `NDVI_implementation/NDVI_Semana5_final.ipynb`: notebook final em portugues.
- `NDVI_implementation/src/`: entrada local (rasters e imagens de apoio).
- `NDVI_implementation/output/`: saidas geradas (`map`, `hist`, `stats`).
- `requirements.txt`: dependencias Python.
- `Semana 5 - Mapeamento de Risco de Inundação e Análise de NDVI.pdf`: enunciado da atividade.

## Como executar
1. Criar e ativar ambiente virtual (opcional).
2. Instalar dependencias:
   ```bash
   pip install -r requirements.txt
   ```
3. Abrir o notebook:
   ```bash
   jupyter notebook NDVI_implementation/NDVI_Semana5_final.ipynb
   ```
4. Ajustar, se necessario, os parametros no topo:
   - `RUN_BASE`
   - `RUN_NEW_REGION`
   - `BASE_RASTER_PATH`
   - `NEW_REGION_RASTER_PATH`

## Saidas esperadas
No diretório `NDVI_implementation/output/`:
- `ndvi_map_base_*.png`
- `ndvi_hist_base_*.png`
- `ndvi_stats_base_*.csv`
- `ndvi_map_new_*.png`
- `ndvi_hist_new_*.png`
- `ndvi_stats_new_*.csv`

## Observacao sobre dados raster
Arquivos `.tif` de Sentinel costumam ultrapassar 100 MB (limite do GitHub).  
Por isso, os `.tif` em `NDVI_implementation/src/` ficam fora do versionamento e devem ser mantidos localmente.

## Entrega recomendada (professor)
- Link do repositorio GitHub com notebook e outputs.
- PDF do relatorio tecnico (3-5 paginas) anexado.
